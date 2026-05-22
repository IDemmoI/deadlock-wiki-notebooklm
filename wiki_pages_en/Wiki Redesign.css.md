# Wiki Redesign.css

/*==== BROWN THEME ====*/
:root {
	--th-html-background-image: url('/images/c/c2/Background_gothic.jpg');
	--th-html-background-color: #3A2D21;
	--th-html-scrollbar: #706F6D #191715;

	--th-mw-body-back: #1e140f;

	--th-p-personal-back: #1f1510;
	--th-p-personal-border: #080504;
	--th-p-personal-a: var(--th-link-color);
	--th-p-personal-a-visited: var(--th-link-color);
	--th-p-personal-a-hover: var(--th-link-color);

	--th-mw-head-list-li-a: #9E8E7C;
	--th-mw-head-list-li-a-select: white;

	--th-mw-head-menu-tabs-li-back: #120b08;
	--th-mw-head-menu-tabs-li-border: #080504;

	--th-mw-head-menu-tabs-li-select-back-1: #453427;
	--th-mw-head-menu-tabs-li-select-back-2: #3D4032;
	--th-mw-head-menu-tabs-li-select-border: #6EA399;

	--th-mw-head-menu-dropdown-head-back: #120b08;
	--th-mw-head-menu-dropdown-head-border: #080504;
	--th-mw-head-menu-dropdown-head: #645b50;

	--th-search-box-inner-back: #1f1510;
	--th-search-box-inner-border: #080504;
	--th-search-box-input-back: rgba(255, 255, 255, 0.1);
	--th-search-box-input: white;
	--th-search-box-input-placeholder: var(--text-color);

	--th-mw-panel-portlet-back: #1F1510;
	
	--th-link-color: #60f8b3 !important;
	--th-alt-link-color: #fff4dfcc !important;
	--th-box-shadow: 2px 2px 5px 0px #0000005e;
}
/*---- custom samlovesmath css starts HERE vvv ----*/
/*===================================*/
/*          DEFAULTS                 */
/*===================================*/
a,
a:visited,
a:hover {
	color: var(--th-link-color);
}

a.new, a.new:visited {
    color: #ff4e4e;
}

a.new:hover {
	color: #ff5a5a;
}

:root {
	--text-color: oklch(0.97 0.03 82.14);
	
    --color-base: var(--text-color);
    --color-base--hover: var(--text-color);
    --color-emphasized: white;
    --color-subtle: #9aa4aa;
    --color-notice: var(--color-subtle);
    --color-content-added: #009c00;
    --color-destructive: #e64835;
    --color-destructive--visited--active: #eb8585;
    --color-progressive--focus: #72a1ff;

    --background-color-base: var(--th-mw-head-menu-dropdown-head-back);
    --background-color-neutral-subtle: var(--th-mw-head-menu-dropdown-head-back);
    --background-color-neutral: var(--th-mw-panel-portlet-back);
    --background-color-interactive-subtle: var(--th-mw-panel-portlet-back);
    --background-color-interactive: var(--th-mw-head-menu-dropdown-head);
    --background-color-content-removed: #CC0000;
    --background-color-content-added: #4ea8f3;

    --background-color-progressive-subtle: var(--th-mw-head-menu-dropdown-head);
    --background-color-disabled: var(--th-mw-body-back);
    
    --background-color-disabled-subtle: var(--th-mw-body-back);
    --background-color-warning-subtle: var(--th-mw-head-menu-dropdown-head);
    --background-color-error-subtle: var(--th-mw-head-menu-dropdown-head);
    --background-color-success-subtle: var(--th-mw-head-menu-dropdown-head);
    --background-color-notice-subtle: var(--th-mw-head-menu-dropdown-head);
    

    --border-color-base: var(--th-mw-head-menu-dropdown-head);
    --border-color-subtle: var(--th-mw-head-menu-dropdown-head);
    --border-color-muted: var(--th-mw-head-menu-dropdown-head);
    --border-color-disabled: var(--th-mw-head-menu-dropdown-head);
}

/*===================================*/
/*          MAIN BODY                */
/*===================================*/
html {
	position: relative;
	background: var(--th-html-background-color);
	scrollbar-color: var(--th-html-scrollbar);
}

/*.parasoid-body ? */
.mw-body {
    background-color: var(--th-mw-body-back);
    color: var(--text-color);
    direction: ltr;
    padding: 1.25em 1.5em 1.5em 1.5em;
    margin-right: 15px;
    border: 2px solid #080504;
    box-shadow: var(--th-box-shadow);
}

.mw-heading,
h1,
h2,
h3,
h4,
h5,
h6 {
	color: var(--text-color);
}

/*===================================*/
/*          HEADER                   */
/*===================================*/
#mw-page-base {
	background: none;
}

.skin-vector-legacy #pt-notifications-notice .mw-echo-notifications-badge,
.skin-vector-legacy #pt-notifications-alert .mw-echo-notifications-badge {
	top: 0;
	width: 14px;
	height: 14px;
	background-size: 14px 14px;
	margin-right: 8px;
}

.skin-vector-legacy #pt-notifications-notice .mw-echo-notifications-badge,
.skin-vector-legacy #pt-notifications-alert .mw-echo-notifications-badge {
	top: 0;
	width: 14px;
	height: 14px;
	background-size: 14px 14px;
	margin-right: 0px
}

#p-personal {
	background-color: var(--th-p-personal-back);
	padding: 0.5em;
	border: 2px solid var(--th-mw-head-menu-tabs-li-border);
	box-shadow: var(--th-box-shadow);
	right: calc(1em + -1px);
}

.vector-user-menu-legacy li {
	font-size: 0.75em;
	float: left;
	margin-left: 0;
	padding-top: 0;
	line-height: 1.16666667;
}

body:not(.skin-vector-2022) #pt-notifications-alert .mw-echo-notifications-badge.mw-echo-notifications-badge-all-read,
body:not(.skin-vector-2022) #pt-notifications-notice .mw-echo-notifications-badge.mw-echo-notifications-badge-all-read {
	opacity: 1
}

.skin-vector-legacy #p-personal #pt-notifications-alert,
.skin-vector-legacy #p-personal #pt-notifications-notice {
	margin-right: 0;
}

.vector-user-menu-legacy #pt-anonuserpage,
.vector-user-menu-legacy #pt-userpage a,
#pt-uls .uls-trigger,
.skin-vector-legacy #pt-uls .uls-trigger {
	padding-top: 0 !important
}

.vector-user-menu-legacy .vector-menu-content-list {
	display: flex;
	flex-wrap: wrap;
	flex-grow: 1;
	flex-direction: row;
	gap: 0.7em;
	align-items: center;
}

@media screen {
	#p-personal a {
		color: var(--th-alt-link-color);
	}
	#p-personal a:visited {
		color: var(--th-alt-link-color);
	}
	#p-personal a:hover {
		color: var(--th-alt-link-color);
	}
}

#p-personal ul {
	padding-left: 0em;
}

/* ---------------- TABS --------------------*/
#mw-head > div .vector-menu-tabs-legacy,
#mw-head > div .vector-menu-dropdown {
	height: 2em;
	margin-top: 0.5em;
}

#mw-head > div .vector-menu-tabs {
	background-image: none;
}

.vector-menu-content-list {
	right: 1px;
    position: relative;
}

#mw-head > div .vector-menu-tabs-legacy ul {
	height: 2em;
	/*-3px*/
}

#mw-head > div .vector-menu-content-list > li:not(:first-child),
#mw-head > div > nav:not(:first-child) {
	margin-left: 0.2em;
}

#p-cactions .vector-menu-content-list {
	background-color: var(--th-mw-panel-portlet-back);
}
#p-cactions .vector-menu-content-list > li {
    margin-left: 0 !important;
}

#mw-head > div .vector-menu-content-list > li.selected {
	margin-bottom: -1px;
}

#mw-head > div .vector-menu-content-list > li > a {
	padding-top: calc(0.65em - 2px);
	padding-left: 11px;
	padding-right: 11px;
	height: 100%;
	background-image: none;
	color: var(--th-alt-link-color);
}

#ca-watch.icon a,
#ca-unwatch.icon a#ca-watch.icon a,
#ca-unwatch.icon a {
	padding-left: 6px !important;
	padding-right: 6px !important;
}

#mw-head > div .vector-menu-tabs-legacy li:hover {
	background-color: var(--th-mw-body-back)
}

#mw-head > div .vector-menu-content-list > li.selected > a {
	padding-top: calc(0.65em - 2px);
	background-image: none;
	color: var(--th-mw-head-list-li-a-select);
}

.vector-user-menu-legacy #pt-userpage a {
    background-repeat: no-repeat;
    background-size: 20px 20px;
    background-position: left 50%;
    padding-left: 2em;
    padding-top: 2px;
    background-image: url(./Special:FilePath/Abrams.png); /* Default */
}
    
.skin-vector-legacy #pt-uls .uls-trigger::before{
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' viewBox='0 0 20 20'%3E%3Cpath fill='%23fff4df' d='M20 18h-1.44a.61.61 0 0 1-.4-.12.81.81 0 0 1-.23-.31L17 15h-5l-1 2.54a.77.77 0 0 1-.22.3.59.59 0 0 1-.4.14H9l4.55-11.47h1.89zm-3.53-4.31L14.89 9.5a11.62 11.62 0 0 1-.39-1.24q-.09.37-.19.69l-.19.56-1.58 4.19zm-6.3-1.58a13.43 13.43 0 0 1-2.91-1.41 11.46 11.46 0 0 0 2.81-5.37H12V4H7.31a4 4 0 0 0-.2-.56C6.87 2.79 6.6 2 6.6 2l-1.47.5s.4.89.6 1.5H0v1.33h2.15A11.23 11.23 0 0 0 5 10.7a17.19 17.19 0 0 1-5 2.1q.56.82.87 1.38a23.28 23.28 0 0 0 5.22-2.51 15.64 15.64 0 0 0 3.56 1.77zM3.63 5.33h4.91a8.11 8.11 0 0 1-2.45 4.45 9.11 9.11 0 0 1-2.46-4.45z'/%3E%3C/svg%3E");
    opacity: 1;
    }
    
.oo-ui-icon-tray, .mw-ui-icon-tray::before {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' viewBox='0 0 20 20'%3E%3Cpath fill='%23fff4df' d='M3 1a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V3a2 2 0 0 0-2-2zm14 12h-4l-1 2H8l-1-2H3V3h14z'/%3E%3C/svg%3E");
}
    
.oo-ui-icon-bell, .mw-ui-icon-bell::before {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' viewBox='0 0 20 20'%3E%3Cpath fill='%23fff4df' d='M16 7a5.38 5.38 0 0 0-4.46-4.85C11.6 1.46 11.53 0 10 0S8.4 1.46 8.46 2.15A5.38 5.38 0 0 0 4 7v6l-2 2v1h16v-1l-2-2zm-6 13a3 3 0 0 0 3-3H7a3 3 0 0 0 3 3'/%3E%3C/svg%3E");
    opacity: 1 !important;
}  

/* colorize */
#mw-head > div .vector-menu-tabs-legacy li {
	height: calc(100% - 3px);
	background-image: none;
	background-color: var(--th-mw-head-menu-tabs-li-back);
	border: 2px solid var(--th-mw-head-menu-tabs-li-border);
	position: relative;
	top: 2px;
	border-bottom-width: 0px;
}

#mw-head > div .vector-menu-tabs-legacy li.selected {
	background: var(--th-mw-body-back);
	border: 2px solid #080504;
	border-bottom-width: 0px;
}

#mw-head > div .vector-menu-dropdown .vector-menu-heading {
	position: relative !important;
	top: 2px !important;
	border-bottom-width: 0 !important;
}

/* watch icon */
#ca-watch.icon a span,
#ca-unwatch.icon a span {
	display: none !important;
}

#ca-watch.icon a,
#ca-unwatch.icon a {
	text-indent: -9999px;
	white-space: nowrap;
	overflow: hidden;
}
    
.vector-menu-tabs .mw-watchlink.icon a::before{
    top: auto;
    left: auto;
}

.vector-menu-tabs #ca-watch.icon a::before {
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16'%3E%3Cpath fill='none' stroke='%23ffffff' stroke-width='1.2' d='M8 1.2 9.9 5.2l4.4.6-3.2 3.1.8 4.3L8 11.2l-3.9 2 0.8-4.3L1.7 5.8l4.4-.6z'/%3E%3C/svg%3E");
}

.vector-menu-tabs #ca-watch.icon a:hover::before,
.vector-menu-tabs #ca-watch.icon a:focus::before {
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16'%3E%3Cpath fill='%237cdaa1' stroke='%237cdaa1' d='M8 1.2 9.9 5.2l4.4.6-3.2 3.1.8 4.3L8 11.2l-3.9 2 0.8-4.3L1.7 5.8l4.4-.6z'/%3E%3C/svg%3E");
}

.vector-menu-tabs #ca-unwatch.icon a::before {
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16'%3E%3Cpath fill='%237cdaa1' stroke='%237cdaa1' d='M8 1.2 9.9 5.2l4.4.6-3.2 3.1.8 4.3L8 11.2l-3.9 2 0.8-4.3L1.7 5.8l4.4-.6z'/%3E%3C/svg%3E");
}

.vector-menu-tabs #ca-unwatch.icon a:hover::before,
.vector-menu-tabs #ca-unwatch.icon a:focus::before {
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16'%3E%3Cpath fill='none' stroke='%23ffffff' stroke-width='1.2' d='M8 1.2 9.9 5.2l4.4.6-3.2 3.1.8 4.3L8 11.2l-3.9 2 0.8-4.3L1.7 5.8l4.4-.6z'/%3E%3C/svg%3E");
}

.vector-menu-tabs #ca-watch.icon a:focus::before,
.vector-menu-tabs #ca-unwatch.icon a:focus::before {
    box-shadow: 0 0 0 2px rgba(124, 218, 161, 0.35);
    border-radius: 2px;
}   

/* more dropdown */
#mw-head > div .vector-menu-dropdown .vector-menu-heading {
	padding-top: calc(0.65em - 2px);
	padding-left: 6px;
	padding-right: 6px;
	height: calc(1.35em - 1px);

	background-color: var(--th-mw-head-menu-dropdown-head-back);
	background-image: none;
	border: 2px solid var(--th-mw-head-menu-dropdown-head-border);
	color: var(--th-alt-link-color);
}

#mw-head > div .vector-menu-dropdown .vector-menu-heading::after {
	background: url('data:image/svg+xml,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22UTF-8%22%3F%3E%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20width%3D%2212%22%20height%3D%2212%22%20viewBox%3D%220%200%2012%2012%22%3E%3Cpath%20fill%3D%22%23645b50%22%20d%3D%22m11.05%203.996-.965-1.053-4.035%203.86-3.947-3.86L1.05%203.996l5%205z%22%2F%3E%3C%2Fsvg%3E') 100% 60% no-repeat;
}

/*===================================*/
/*          NAVIGATION               */
/*===================================*/

.vector-legacy-sidebar .vector-menu-portal .vector-menu-heading {
	background-image: none !important;
	background: var(--th-mw-head-menu-dropdown-head-back);
	padding: 0.3em 0.6em;
	font-size: 16px;
	font-family: 'VALVE Pulp';
	font-variant: small-caps;
	color: var(--text-color);
	margin:unset !important;
}

.vector-legacy-sidebar .vector-menu-portal .vector-menu-content li a,
.vector-legacy-sidebar .vector-menu-portal .vector-menu-content li a:visited {
	color: var(--th-alt-link-color) !important;
}

#mw-panel.vector-legacy-sidebar > nav.mw-portlet {
    padding: 0.4em 0.3em;
    margin: 0 0 0.5em 0;
    background-color: var(--th-mw-panel-portlet-back);
    border: 2px solid var(--th-mw-head-menu-tabs-li-border);
    box-shadow: 2px 2px 5px 0px #0000005e;
}

.skin-vector-legacy #pt-uls .uls-trigger::before {
    top: 2px;
    position:relative;
}

.vector-legacy-sidebar .vector-menu-portal .vector-menu-heading {
	background-image: none !important
}

#p-logo + .mw-portlet .vector-menu-heading {
	display: block !important;
}

#p-logo {
	margin-bottom: 0;
}

#mw-indicator-protection-moderator {
	display: none
}

/*===================================*/
/*          LOGO                     */
/*===================================*/

.mw-wiki-logo {
    background-image: url(/images/thumb/7/70/Deadlock_Wiki.png/250px-Deadlock_Wiki.png);
    background-size: contain;
}

/*===================================*/
/*          BODY STUFF               */
/*===================================*/
/* changes for editor window */
.wikiEditor-ui-toolbar ::before,
.wikiEditor-ui-toolbar .oo-ui-buttonElement-button{
    filter: brightness(0) invert(1) !important;
}

.mw-parser-output a.external,
.mw-parser-output a.external:visited,
.mw-parser-output a.extiw:visited,
.mw-parser-output a.extiw{
    color: var(--th-link-color);
}

.mw-parser-output a.external,
.mw-parser-output a.external:visited{
	background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 12 12'%3E%3Cpath fill='%237cdaa1' d='M6 1h5v5L8.86 3.85 4.7 8 4 7.3l4.15-4.16zM2 3h2v1H2v6h6V8h1v2a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V4a1 1 0 0 1 1-1'/%3E%3C/svg%3E");
}

/* remove header if main page */
#firstHeading:has( + #bodyContent > #mw-content-text > .mw-content-ltr > div > div > .mainpage-header) {
	display: none;
}

/* remove bottom line from header if deadlock navigation table is present */
#content:has( #mw-content-text > div.mw-parser-output:first-child > .deadlock-nav-table:first-child) h1#firstHeading {
	border-bottom: none;
	margin-bottom: 0px;
}

.module-icon-ability {
	filter: none !important:
}

/* TOC styling */
.tocnumber {
  color: var(--text-color);
}

.toc,
.toccolours {
  background-color: var(--th-mw-head-menu-dropdown-head-back);
  border: 1px solid var(--th-mw-head-menu-tabs-li-border);
}

.toctogglelabel {
  color: var(--th-link-color);
  cursor: pointer;
}

.toctitle,
.toctitle h2 {
	font-family: 'Retail Demo' !important;
}
/* TOC styling */

.oo-ui-windowManager-modal > .oo-ui-dialog > .oo-ui-window-frame{
	background-color: var(--th-mw-body-back);
}

.oo-ui-window-content .oo-ui-processDialog-title,
.oo-ui-window-content .oo-ui-layout span {
    color: var(--text-color);
}

.oo-ui-indicatorElement-indicator,
.oo-ui-window-content .oo-ui-icon-tag,
.oo-ui-iconElement-icon {
    filter: brightness(0) invert(1) !important;
}

.oo-ui-checkboxInputWidget-checkIcon,
.editCheckboxes .oo-ui-iconElement-icon {
    filter: none !important;
}

.mw-collapsible-toggle-default .mw-collapsible-text{
	color: var(--th-link-color);
}

.mw-collapsible-toggle-default::before,
.mw-collapsible-toggle-default::after{
    color: var(--text-color);        
}

@media screen {
  ul {
    list-style-image: none !important;
  }
}
    
ul {
    list-style-type: disc;
  }

ul li::marker {
  color: var(--text-color);
}

.mwe-popups .mwe-popups-extract[dir="ltr"]::after {
  right: 0;
  background-image: linear-gradient(to right,rgba(255,255,255,0), var(--th-mw-head-menu-dropdown-head-back) 50%);
}

.uls-menu, .uls-search, .uls-lcd, #uls-settings-block{
    background-color: var(--th-mw-body-back);
}

.uls-language-block > ul > li:hover{
    background-color: var(--th-mw-head-menu-dropdown-head-back);
}

.uls-filtersuggestion{
    background-color: var(--th-search-box-inner-back);
}
.uls-menu .uls-no-results-view h3,
.uls-no-found-more,
.uls-no-results-found-title,
.skin-vector .uls-languagefilter, .skin-vector .uls-lcd-region-title{
    color: var(--text-color);
}

.uls-no-found-more{
    border-top: 1px solid var(--th-search-box-inner-border);
}
.uls-language-block a{
    color: var(--th-link-color);
}

.mw-json-value, .mw-json-single-value{
	background-color: var(--th-html-background-color);
}

/* Changes for code editor (css, js, json, etc.) */
/* Base */
.mw-highlight {
  background: #1F1510;
  color: #E8DED6;
}

.mw-highlight pre,
.mw-highlight code {
  background: transparent;
  color: inherit;
}

/* highlighted line */
.mw-highlight .hll {
  background-color: rgba(255, 184, 108, 0.12);
}

/* line numbers (if enabled by the highlighter) */
.mw-highlight .linenos,
.mw-highlight .lineno {
  background: #17110E;
  color: #A89A90;
  padding: 0 0.6em;
  z-index: 0;
}

/* whitespace */
.mw-highlight .w {
  color: #5C4C44;
}

/* errors / invalid */
.mw-highlight .err {
  background-color: rgba(255, 80, 80, 0.15);
  color: #FF8A8A;
  border: 1px solid rgba(255, 107, 107, 0.55);
}

/* comments */
.mw-highlight .c,
.mw-highlight .ch,
.mw-highlight .cm,
.mw-highlight .cpf,
.mw-highlight .c1,
.mw-highlight .cs {
  color: #A89A90;
  font-style: italic;
}

/* preprocessor / directive-ish comments */
.mw-highlight .cp {
  color: #B8ADA6;
  font-style: italic;
}

/* keywords */
.mw-highlight .k,
.mw-highlight .kc,
.mw-highlight .kd,
.mw-highlight .kn,
.mw-highlight .kr,
.mw-highlight .kp {
  color: #7EE787;
  font-weight: bold;
}

/* keyword: type */
.mw-highlight .kt {
  color: #B8A1FF;
  font-weight: bold;
}

/* operators + punctuation */
.mw-highlight .o,
.mw-highlight .ow,
.mw-highlight .p {
  color: #D0C7C0;
}

/* numbers */
.mw-highlight .m,
.mw-highlight .mb,
.mw-highlight .mf,
.mw-highlight .mh,
.mw-highlight .mi,
.mw-highlight .mo,
.mw-highlight .il {
  color: #F2C38B;
}

/* strings */
.mw-highlight .s,
.mw-highlight .sa,
.mw-highlight .sb,
.mw-highlight .sc,
.mw-highlight .dl,
.mw-highlight .s2,
.mw-highlight .sh,
.mw-highlight .s1,
.mw-highlight .sx,
.mw-highlight .ss {
  color: #FFB86C;
}

/* docstrings */
.mw-highlight .sd {
  color: #B8ADA6;
  font-style: italic;
}

/* string escapes / interpolation */
.mw-highlight .se,
.mw-highlight .si {
  color: #F2C38B;
}

/* regex */
.mw-highlight .sr {
  color: #FF6B6B;
}

/* names / identifiers (more Ace-like mapping) */
.mw-highlight .n {
  color: #E8DED6;
}

/* functions */
.mw-highlight .nf,
.mw-highlight .fm {
  color: #8BE9FD;
}

/* variables */
.mw-highlight .nv,
.mw-highlight .vc,
.mw-highlight .vg,
.mw-highlight .vi,
.mw-highlight .vm {
  color: #8BE9FD;
}

/* builtins / pseudo-builtin */
.mw-highlight .nb,
.mw-highlight .bp {
  color: #8BE9FD;
}

/* constants */
.mw-highlight .no,
.mw-highlight .nc /* (if your lexer emits class names as constants in some modes) */ {
  color: #F2C38B;
}

/* classes / types / namespaces */
.mw-highlight .nc,
.mw-highlight .nn {
  color: #B8A1FF;
}

/* exceptions */
.mw-highlight .ne {
  color: #FF6B6B;
}

/* decorators / annotations */
.mw-highlight .nd {
  color: #7AA2F7;
}

/* labels */
.mw-highlight .nl {
  color: #7EE787;
}

/* XML/HTML tags & attributes */
.mw-highlight .nt {
  color: #7AA2F7;
}

.mw-highlight .na {
  color: #F2C38B;
}

/* entities */
.mw-highlight .ni {
  color: #D0C7C0;
}

/* generic / headings / emphasis */
.mw-highlight .gh,
.mw-highlight .gu,
.mw-highlight .gp {
  color: #B8A1FF;
  font-weight: bold;
}

/* deleted / inserted */
.mw-highlight .gd {
  color: #FF6B6B;
}

.mw-highlight .gi {
  color: #7EE787;
}

/* generic output / tracebacks */
.mw-highlight .go {
  color: #B8ADA6;
}

.mw-highlight .gt {
  color: #7AA2F7;
}

.cm-mw-template-name, .cm-mw-template-argument-name, .cm-mw-template-delimiter, .cm-mw-template-bracket {
    color: #d47fff;
}

.ace-tm {
  background-color: #1F1510;
  color: #E8DED6;
}

/* gutter */
.ace-tm .ace_gutter {
  background: #17110E;
  color: #A89A90;
}

/* print margin */
.ace-tm .ace_print-margin {
  width: 1px;
  background: #2C201B;
}

/* fold marker */
.ace-tm .ace_fold {
  background-color: #7AA2F7;
}

/* cursor */
.ace-tm .ace_cursor {
  color: #F2E9E4;
}

/* invisible chars */
.ace-tm .ace_invisible {
  color: #5C4C44;
}

/* keywords */
.ace-tm .ace_storage,
.ace-tm .ace_keyword {
  color: #7EE787;
}

/* constants */
.ace-tm .ace_constant {
  color: #F2C38B;
}

.ace-tm .ace_constant.ace_buildin {
  color: #8BE9FD;
}

.ace-tm .ace_constant.ace_language {
  color: #7AA2F7;
}

.ace-tm .ace_constant.ace_library {
  color: #7EE787;
}

/* invalid */
.ace-tm .ace_invalid {
  background-color: rgba(255, 80, 80, 0.15);
  color: #FF8A8A;
}

/* functions */
.ace-tm .ace_support.ace_function {
  color: #8BE9FD;
}

.ace-tm .ace_support.ace_constant {
  color: #7EE787;
}

.ace-tm .ace_support.ace_type,
.ace-tm .ace_support.ace_class {
  color: #B8A1FF;
}

/* operators */
.ace-tm .ace_keyword.ace_operator {
  color: #D0C7C0;
}

/* strings */
.ace-tm .ace_string {
  color: #FFB86C;
}

/* comments */
.ace-tm .ace_comment {
  color: #A89A90;
  font-style: italic;
}

.ace-tm .ace_comment.ace_doc {
  color: #B8ADA6;
}

.ace-tm .ace_comment.ace_doc.ace_tag {
  color: #8C7A70;
}

/* numbers */
.ace-tm .ace_constant.ace_numeric {
  color: #F2C38B;
}

/* variables */
.ace-tm .ace_variable {
  color: #8BE9FD;
}

/* XML / markup */
.ace-tm .ace_xml-pe {
  color: #A89A90;
}

.ace-tm .ace_meta.ace_tag {
  color: #7AA2F7;
}

/* regex */
.ace-tm .ace_string.ace_regex {
  color: #FF6B6B;
}

/* selection */
.ace-tm .ace_marker-layer .ace_selection {
  background: rgba(122, 162, 247, 0.25);
}

.ace-tm.ace_multiselect .ace_selection.ace_start {
  box-shadow: 0 0 3px 0px #F2E9E4;
}

/* active line / step / stack */
.ace-tm .ace_marker-layer .ace_step {
  background: rgba(255, 184, 108, 0.25);
}

.ace-tm .ace_marker-layer .ace_stack {
  background: rgba(126, 231, 135, 0.18);
}

.ace-tm .ace_marker-layer .ace_active-line {
  background: rgba(255, 255, 255, 0.04);
}

/* brackets */
.ace-tm .ace_marker-layer .ace_bracket {
  margin: -1px 0 0 -1px;
  border: 1px solid #5C4C44;
}

/* gutter active line */
.ace-tm .ace_gutter-active-line {
  background-color: #241A16;
  color: #E8DED6;
}

/* selected word */
.ace-tm .ace_marker-layer .ace_selected-word {
  background: rgba(255, 184, 108, 0.12);
  border: 1px solid rgba(255, 184, 108, 0.25);
}

/* indent guides */
.ace-tm .ace_indent-guide {
  background: none;
  border-right: 1px dotted #3A2A24;
}

.ace-tm .ace_indent-guide-active {
  background: none;
  border-right: 1px dotted #5C4C44;
}

/*alert and notices menu*/
.mw-echo-ui-notificationItemWidget:hover {
	text-decoration: none;
	background-color: var(--background-color-base, #fff);
}

.mw-echo-ui-notificationBadgeController-popup > .oo-ui-popupWidget-popup > .oo-ui-popupWidget-head > .oo-ui-labelElement-label {
	color: var(--text-color);
	font-family: 'VALVE Pulp';
}

.oo-ui-labelElement .oo-ui-labelElement-label {
	line-height: 1.42857143em;
	color: var(--text-color);
}

.mw-echo-ui-notificationItemWidget-icon {
    position: absolute;
    filter: invert(1);
    opacity: 0.7;
}

/* Icon options */
body.usericon-abrams .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/e/e0/Abrams.png); }
body.usericon-apollo .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/1/14/Apollo.png); }
body.usericon-bebop .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/4/46/Bebop.png); }
body.usericon-billy .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/9/95/Billy.png); }
body.usericon-calico .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/7/7b/Calico.png); }
body.usericon-celeste .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/4/49/Celeste.png); }
body.usericon-doorman .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/a/ae/The_Doorman.png); }
body.usericon-drifter .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/8/89/Drifter.png); }
body.usericon-dynamo .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/0/05/Dynamo.png); }
body.usericon-graves .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/6/66/Graves.png); }
body.usericon-grey-talon .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/8/8b/Grey_Talon.png); }
body.usericon-haze .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/e/e8/Haze.png); }
body.usericon-holliday .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/7/7a/Holliday.png); }
body.usericon-infernus .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/d/d2/Infernus.png); }
body.usericon-ivy .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/3/3f/Ivy.png); }
body.usericon-kelvin .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/2/22/Kelvin.png); }
body.usericon-lady-geist .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/a/a9/Lady_Geist.png); }
body.usericon-lash .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/b/bb/Lash.png); }
body.usericon-mcginnis .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/d/da/McGinnis.png); }
body.usericon-mina .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/6/6b/Mina.png); }
body.usericon-mirage .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/f/fb/Mirage.png); }
body.usericon-mo-krill .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/e/e5/Mo_%26_Krill.png); }
body.usericon-paige .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/2/2f/Paige.png); }
body.usericon-paradox .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/b/b0/Paradox.png); }
body.usericon-pocket .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/e/ee/Pocket.png); }
body.usericon-rem .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/4/4b/Rem.png); }
body.usericon-rem-helper .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/c/c5/Rem_helper.png); }
body.usericon-seven .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/f/fe/Seven.png); }
body.usericon-shiv .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/b/b6/Shiv.png); }
body.usericon-silver .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/0/0b/Silver.png); }
body.usericon-sinclair .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/5/54/Sinclair.png); }
body.usericon-venator .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/d/db/Venator.png); }
body.usericon-victor .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/9/90/Victor.png); }
body.usericon-vindicta .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/f/f3/Vindicta.png); }
body.usericon-viscous .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/e/e9/Viscous.png); }
body.usericon-vyper .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/2/2f/Vyper.png); }
body.usericon-warden .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/a/a5/Warden.png); }
body.usericon-wraith .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/7/7c/Wraith.png); }
body.usericon-yamato .vector-user-menu-legacy #pt-userpage a { background-image: url(./images/6/64/Yamato.png); }

/* Selector styling */
#usericon-selector {
    background: var(--th-mw-panel-portlet-back);
    border: 1px solid var(--th-mw-head-menu-dropdown-head);
    padding: 15px;
    margin: 15px 0;
    border-radius: 4px;
}

#usericon-selector h3 {
    margin-top: 0;
    color: var(--color-emphasized);
}

.usericon-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
    gap: 10px;
    margin-top: 10px;
}

.usericon-option {
    cursor: pointer;
    border: 3px solid transparent;
    padding: 5px;
    text-align: center;
    border-radius: 4px;
    transition: all 0.2s;
    background: var(--th-mw-head-menu-dropdown-head-back);
}

.usericon-option:hover {
    border-color: var(--th-mw-head-menu-dropdown-head);
    background: var(--background-color-interactive);
}

.usericon-option.selected {
    border-color: var(--th-link-color);
    background: var(--th-mw-head-menu-tabs-li-select-back-1);
    box-shadow: 0 0 8px rgba(124, 218, 161, 0.3);
}

.usericon-option img {
    width: 64px;
    height: 64px;
    display: block;
    margin: 0 auto 5px;
    border-radius: 2px;
}

.usericon-option span {
    display: block;
    font-size: 0.9em;
    color: var(--text-color);
}

.usericon-option.selected span {
    color: var(--color-emphasized);
    font-weight: bold;
}

#usericon-selector.collapsed .usericon-grid {
    display: none;
}

.usericon-toggle {
    cursor: pointer;
    user-select: none;
}

.usericon-toggle:hover {
    opacity: 0.8;
}

.usericon-toggle-icon {
    display: inline-block;
    width: 1em;
}

.usericon-toggle {
    padding-top: 0;
}

.usericon-option.infected {
animation: infectedPulseOnce 0.6s ease-out;
}

@keyframes infectedPulseOnce {
    0% {
        transform: scale(1);
        filter: brightness(1);
    }
    50% {
        transform: scale(1.15);
        filter: brightness(1.25);
    }
    100% {
        transform: scale(1);
        filter: brightness(1);
    }
}

#pt-uls {
	display: none;
}

#left-navigation, #right-navigation, #content {
	position: relative;
	top:0.6em;
}

/* Main layout width control */
body {
    max-width: var(--fixed-width);
    margin: auto;
    background: none;
    width: 100%;
	height: 100vh
}

body::after {
	content: "";
	position: fixed;
	inset: 0;
	z-index: -1;
	background-color: var(--th-html-background-color);
	mix-blend-mode: color; /* remove this for full color image */
}

body::before {
	content: "";
	position: absolute;
	inset: 0;
	z-index: -1;
	background-image: linear-gradient(#0000, var(--th-html-background-color) 60%), var(--th-html-background-image);
	background-position: top center, top center;
	background-size: cover, cover;
	background-repeat: no-repeat, no-repeat;
	background-attachment: scroll, scroll;
}

/* Header alignment */
#mw-head {
	max-width: var(--fixed-width);
	right: unset;
}

/* Sidebar positioning */
#mw-panel {
	left: unset;
}

/* Search box scaling */
.vector-search-box-inner,
#p-search #searchform .cdx-search-input__input-wrapper {
	width: min(20vw, calc(var(--fixed-width) / 5));
}

/* Notifications positioning */
body .mw-notification-area {
	right: calc(50% - min(50%, var(--fixed-width) / 2));
}

/* Page base adjustment */
div#mw-page-base::after {
	position: relative;
	display: block;
	width: 0;
	right: calc(16px - min(100%, var(--fixed-width)));
}

#pt-fixedwidth-toggle a {
    width: 14px;
    height: 14px;
    display: block;
    opacity: 0.6;
    background: var(--color-base);
    mask-clip: inherit;
    mask-image: url(/load.php?format=original&image=fullScreen&variant=invert&modules=oojs-ui.styles.icons-media&skin=vector);
    mask-size: 14px 14px;
}

#pt-fixedwidth-toggle a:hover {
	opacity: 1;
}

/* search bar */
.cdx-text-input__input:enabled,
.cdx-text-input__input:hover,
.cdx-text-input__input:enabled:hover,
.cdx-text-input__input:enabled:focus,
.cdx-text-input__input:enabled:focus:hover,
.cdx-search-input--has-end-button .cdx-search-input__input-wrapper .cdx-text-input,
.cdx-search-input--has-end-button,
.cdx-search-input__input-wrapper,
.cdx-text-input,
.cdx-text-input__input {
	border: transparent 0px solid !important;
	color: #ffffffb3 !important;
	box-shadow: unset !important;
	border-radius: 0px !important;
}

.cdx-text-input__input:enabled {
	background-color: var(--th-mw-body-back) !important;
}

.vector-search-box .cdx-search-input__end-button.cdx-button {
	filter: invert(1);
	opacity: 0.5 !important
}

.cdx-search-input__input-wrapper {
	border-color: var(--th-mw-head-menu-tabs-li-border) !important;
	border-style: solid !important;
	border-top-width: 2px !important;
	border-right-width: 2px !important;
	border-bottom-width: 0 !important;
	border-left-width: 2px !important;
}

input::placeholder {
	color: var(--text-color) !important;
	opacity: 0.5 !important;
}

.cdx-menu-item--enabled.cdx-menu-item--highlighted {
	background-color: #ffffff17 !important
}

#p-search {
	margin-right: 16px;
	top: 2px;
	position: relative
}

/* STUPID FUCKING MOBILE MINERVA DOGSHIT */
@media (max-width: 600px) {

	#left-navigation,
	#right-navigation,
	#content {
		position: relative;
		top: 0;
		margin: 0;
		border: unset
	}

	.mw-body {
		padding: 0;
		margin: 0
	}

	.header-container.header-chrome {
		background-color: var(--background-color-interactive, #eaecf0);
		border: 0;
		box-shadow: inset 0 -1px 3px rgba(0, 0, 0, 0.08);
		background-image: url(https://deadlock.wiki/images/3/39/News_shop_rework_png.webp);
		background-size: 50em;
		background-position: top center;
	}

	.minerva-icon,
	.cdx-button:hover,
	.cdx-button:active,
	.cdx-button:focus {
		background: #fdfdfd !important;
		opacity: var(--opacity-icon-subtle) !important;
		border: 0 transparent solid !important;
		box-shadow: unset !important
	}

	:root {
		--opacity-icon-subtle: 0.8
	}

	.action-edit .mw-first-heading {
		margin-top: 0;
		padding-top: 0.5em
	}

	.cdx-button:enabled.cdx-button--weight-quiet:active,
	.cdx-button.cdx-button--fake-button--enabled.cdx-button--weight-quiet:active,
	.cdx-button:enabled.cdx-button--weight-quiet.cdx-button--is-active,
	.cdx-button.cdx-button--fake-button--enabled.cdx-button--weight-quiet.cdx-button--is-active,
	.cdx-button:enabled.cdx-button--weight-quiet,
	.cdx-button.cdx-button--fake-button--enabled.cdx-button--weight-quiet {
		background: transparent !important;
		mix-blend-mode: unset !important
	}

	.toggle-list-item__label {
		color: var(--color-base)
	}

	#mw-mf-page-left ul .toggle-list-item .toggle-list-item__anchor:hover {
		box-shadow: inset 4px 0 0 0 var(--color-base)
	}

	.minerva__tab-container .minerva__tab.selected {
		border-bottom: 2px solid #92e3b2;
	}

	.minerva__tab-container .minerva__tab .minerva__tab-text {
		color: #92e3b2
	}

	.minerva__tab-container .minerva__tab .minerva__tab-text,
	.minerva__tab-container .minerva__tab.selected {
		opacity: var(--opacity-icon-subtle)
	}
	
	.page-Deadlock_Wiki .page-heading {
		margin: 0;
	}

	.page-Deadlock_Wiki .heading-holder {
		padding: 5px 0 5px 0;
		position: relative;
	}

	.page-Deadlock_Wiki #firstHeading,
	.page-Deadlock_Wiki #p-associated-pages {
		display: none
	}
	
	.mw-echo-ui-notificationItemWidget {
		background-color: var(--th-mw-head-menu-dropdown-head)
	}
	
	.mw-echo-ui-notificationItemWidget-content-message-header {
		color: var(--text-color) !important
	}
	
	.mw-echo-ui-notificationItemWidget:hover {
		background-color: var(--th-mw-head-menu-dropdown-head)
	}
	
	#p-personal {
		padding: 0;
		background-color: var(--background-color-interactive, #eaecf0);
		border: none;
		box-shadow: none
	}
	
	#mw-mf-page-left ul {
		padding-bottom: 2px;
		padding-right: 1px;
	}
	
    .last-modified-bar__text {
        color: var(--th-link-color);
        opacity: 0.7;
    }
    
    .oo-ui-buttonElement-framed.oo-ui-widget-enabled.oo-ui-flaggedElement-primary.oo-ui-flaggedElement-progressive > .oo-ui-buttonElement-button{
    background-color: var(--th-link-color);
    }
    
    .oo-ui-flaggedElement-progressive.oo-ui-labelElement .oo-ui-labelElement-label{
    	color:black;
    }
}

.content .mw-index-pager-list-header, .mw-special-Watchlist .content h4{
	color:inherit;
}

.mw-mf-amc-disabled.action-history #pagehistory li .history-user a{
	color:var(--th-link-color);
}

.editCheckboxes {
	margin-bottom: 5px;
}

#wpSave {
	color:black;
}

.cm-mw-htmltag-attribute-value {
	color:var(--background-color-content-added);
}

.oo-ui-labelElement-label {
    color: var(--color-base);
}

.wikitable img {
    max-width: 100%;
    height: auto;
}

/* DISCORD NAVIGATION BUTTON */

/* Primary button appearance */
#n-Discord a {
    display: block;
    padding: 6px 10px 5px 32px;
    color: #ffffff !important;
    font-size: 12px;
    font-weight: bold;
    text-align: center;
    text-decoration: none;
    background-color: #6f6658;
    border-radius: 5px;
    border-width: 1px;
    border-style: solid;
    border-color: #91846e #3c372e #3c372e #91846e;
    box-shadow: 1px 1px 3px 0 rgba(0, 0, 0, 0.37);
    transition: background-color 0.2s ease, border-color 0.2s ease;
    position: relative;
    right:-1px;
    margin-bottom: 0.5em;
}

/* Reset default sidebar spacing */
#mw-panel.vector-legacy-sidebar > nav.mw-portlet#p-Discord,
#n-discord,
#p-Discord .vector-menu-content,
#p-Discord .vector-menu-content-list {
    margin: 0;
    padding: 0;
    border: none;
    background: transparent;
    box-shadow: none;
}

/* Hide section heading */
#p-logo + .mw-portlet .vector-menu-heading {
    display: none !important;
}

/* Add text prefix */
#n-Discord a::before {
    content: "Wiki ";
}

/* Discord icon positioning */
#n-Discord a::after {
    content: '';
    position: absolute;
    left: 10px;
    width: 17px;
    height: 13px;
    background-image: url(https://deadlock.wiki/images/4/4c/Discord-Symbol-White.svg);
    background-repeat: no-repeat;
    background-size: 17px 13px;
    filter: drop-shadow(0 1px 1px rgba(0, 0, 0, 0.1));
}

/* Hover state styling */
#n-Discord a:hover {
    background-color: #4f5bdb;
    border-color: #6e78ea #212666 #212666 #6e78ea;
}

.cdx-button:enabled:hover, .cdx-button.cdx-button--fake-button--enabled:hover {
    background-color: #2b1e18;
    border-color: #6e6e6e;
    cursor: pointer;
}

#skin-client-prefs-skin-theme {
	display: none
}

#footer-icons .cdx-button.cdx-button--fake-button--enabled {
    background-color: white;
}

.mw-logevent-actionlink a, .mw-logevent-tool a, .mw-diff-tool a, .mw-pager-tools a {
	color: var(--th-link-color);
}

.diff-deletedline .diffchange {
    background: #cc00005c;
}

.diff-addedline .diffchange {
    background: #4ea8f34f;
}