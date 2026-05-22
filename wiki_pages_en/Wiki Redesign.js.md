# Wiki Redesign.js

/* This page is for editing, actual working JS will be located in [[User:Monster Domosed/Wiki Redesign.js]] 
which you can import with mw.loader.load('https://deadlock.wiki/index.php?title=User:Monster_Domosed/Wiki_Redesign.js&action=raw&ctype=text/javascript'); 
ping [[User:Monster_Domosed]] on Discord if you want your code pushed to working page */

/* Icon selector */
(function () {
    'use strict';

    var availableIcons = [
        { id: 'abrams', name: 'Abrams' },
        { id: 'apollo', name: 'Apollo' },
        { id: 'bebop', name: 'Bebop' },
        { id: 'billy', name: 'Billy' },
        { id: 'calico', name: 'Calico' },
        { id: 'celeste', name: 'Celeste' },
        { id: 'doorman', name: 'The Doorman' },
        { id: 'drifter', name: 'Drifter' },
        { id: 'dynamo', name: 'Dynamo' },
        { id: 'graves', name: 'Graves' },
        { id: 'grey-talon', name: 'Grey Talon' },
        { id: 'haze', name: 'Haze' },
        { id: 'holliday', name: 'Holliday' },
        { id: 'infernus', name: 'Infernus' },
        { id: 'ivy', name: 'Ivy' },
        { id: 'kelvin', name: 'Kelvin' },
        { id: 'lady-geist', name: 'Lady Geist' },
        { id: 'lash', name: 'Lash' },
        { id: 'mcginnis', name: 'McGinnis' },
        { id: 'mina', name: 'Mina' },
        { id: 'mirage', name: 'Mirage' },
        { id: 'mo-krill', name: 'Mo & Krill' },
        { id: 'paige', name: 'Paige' },
        { id: 'paradox', name: 'Paradox' },
        { id: 'pocket', name: 'Pocket' },
        { id: 'rem', name: 'Rem' },
        { id: 'seven', name: 'Seven' },
        { id: 'shiv', name: 'Shiv' },
        { id: 'silver', name: 'Silver' },
        { id: 'sinclair', name: 'Sinclair' },
        { id: 'venator', name: 'Venator' },
        { id: 'victor', name: 'Victor' },
        { id: 'vindicta', name: 'Vindicta' },
        { id: 'viscous', name: 'Viscous' },
        { id: 'vyper', name: 'Vyper' },
        { id: 'warden', name: 'Warden' },
        { id: 'wraith', name: 'Wraith' },
        { id: 'yamato', name: 'Yamato' }
    ];

    var PREFERENCE_KEY = 'userjs-selectedicon';

    var remClickCount = 0;
    var remClickTimer = null;

    var buddyMessages = [
        "I got little buddies.",
        "They cute.",
        "They love.",
        "They help.",
        "They great at shuffleboard.",
        "They do lots of things!",
        "Hi friends!",
        "Come help!",
        "I know you'll help me."
    ];

    function getFilePath(filename) {
        return mw.util.getUrl('Special:FilePath/' + filename);
    }

    function getCachedIcon() {
        return localStorage.getItem(PREFERENCE_KEY);
    }

    function setCachedIcon(iconId) {
        localStorage.setItem(PREFERENCE_KEY, iconId);
    }

    function applyIcon(iconId) {
        document.body.className =
            document.body.className.replace(/usericon-\w+/g, '');
        document.body.classList.add('usericon-' + iconId);
    }

    function applyStoredIcon() {
        var icon = getCachedIcon() || 'rem';

        applyIcon(icon);

        mw.loader.using(['mediawiki.api'], function () {
            var api = new mw.Api();

            api.get({
                action: 'query',
                meta: 'userinfo',
                uiprop: 'options'
            }).done(function (data) {
                var serverIcon =
                    data.query.userinfo.options[PREFERENCE_KEY] || 'rem';

                if (serverIcon !== icon) {
                    setCachedIcon(serverIcon);
                    applyIcon(serverIcon);
                }
            });
        });
    }

    function createIconSelector() {
        var currentIcon = getCachedIcon() || 'rem';

        var html = '<div id="usericon-selector">' +
            '<h3>Choose Your Profile Icon</h3>' +
            '<div class="usericon-grid">';

        availableIcons.forEach(function (icon) {
            var selected = icon.id === currentIcon ? ' selected' : '';
            var imgSrc = getFilePath(icon.name + '.png');

            html += '<div class="usericon-option' + selected + '" data-icon="' + icon.id + '">' +
                '<img src="' + imgSrc + '" alt="' + icon.name + '">' +
                '<span>' + icon.name + '</span>' +
                '</div>';
        });

        html += '</div></div>';

        var $selector = $(html);
        $('#mw-content-text').prepend($selector);

        $('.usericon-option').on('click', function () {
            var iconId = $(this).data('icon');

            if (iconId === 'rem') {
                remClickCount++;

                clearTimeout(remClickTimer);
                remClickTimer = setTimeout(function () {
                    remClickCount = 0;
                }, 1500);

			if (remClickCount >= 5) {
			    remClickCount = 0;
			
			    iconId = 'rem-helper';
			
			    setCachedIcon(iconId);
			    applyIcon(iconId);
			
			    var msg = buddyMessages[Math.floor(Math.random() * buddyMessages.length)];
			
			    mw.notify(msg, {
			        type: 'success'
			    });
			
			    selectIcon(iconId);
			    
                }
            } else {
                remClickCount = 0;
            }

            $('.usericon-option').removeClass('selected');
            $(this).addClass('selected');

            selectIcon(iconId);
        });
    }

    function selectIcon(iconId) {
        var currentIcon = getCachedIcon() || 'rem';

        if (currentIcon === iconId) {
            return;
        }

        setCachedIcon(iconId);
        applyIcon(iconId);

        mw.loader.using(['mediawiki.api'], function () {
            var api = new mw.Api();

            api.saveOption(PREFERENCE_KEY, iconId)
                .done(function () {
                    if (iconId !== 'rem-helper') {
                        mw.notify('Icon updated successfully!', {
                            type: 'success'
                        });
                    }
                })
                .fail(function () {
                    mw.notify('Failed to save icon.', {
                        type: 'error'
                    });
                });
        });
    }

    mw.loader.using(['mediawiki.util'], function () {
        applyStoredIcon();

        var config = mw.config.get([
            'wgNamespaceNumber',
            'wgTitle',
            'wgUserName'
        ]);

        if (
            config.wgNamespaceNumber === 2 &&
            config.wgTitle === config.wgUserName &&
            config.wgUserName
        ) {
            createIconSelector();
        }
    });

})();