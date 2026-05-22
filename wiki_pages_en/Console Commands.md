# Console commands

Console commands allow you to modify gameplay settings. If the player has the "Dev command console" option enabled in settings, pressing **F7** will open the developer console, which allows you to run commands. They can be used in the Hideout, Sandbox and "Explore NYC" modes, as well as cheat-enabled custom games.

For a complete list of console commands and variables, see the Valve Developer Wiki.

## Contents

- 1 Useful Console Commands
- 2 All Known Convars/Commands
- 3 Auto execute console commands on startup
- 4 Hosting Custom Games

- 4.1 Adding Bots
- 5 External links

## Useful Console Commands

[edit | edit source]

Commands that require cheats will not work in standard multiplayer matches. To enable cheats in a custom lobby, run sv_cheats true.

| Command | Values | Default | Description |
| --- | --- | --- | --- |
| bot_kick_all |  |  | Kicks all bots from the game. |
| changelevel | See the map command. |  | Loads a new map.   When used in a multiplayer lobby, players will remain connected while the map changes. |
| changeteam | - 0: Select a team and hero. - 1: Join spectators. - 2: Join The Hidden King and select a hero. - 3: Join The Archmother and select a hero. |  | Allows changing your team and hero. |
| citadel_allow_purchasing_anywhere | true/false |  | Enables purchasing anywhere on the map, not just at shops. Requires cheats. |
| citadel_enable_fast_cooldowns |  |  | Enables fast cooldowns, causing all abilities to have a 2 second cooldown. Requires cheats. |
| citadel_disable_fast_cooldowns |  |  | Disables fast cooldowns. Requires cheats. |
| citadel_enable_fast_stamina |  |  | Enables fast stamina, causing stamina to regen very fast. Requires cheats. |
| citadel_disable_fast_stamina |  |  | Disables fast stamina. Requires cheats. |
| citadel_dps_multiplier | number | 1.0 | Adds a multiplier to player damage output. Affects all damage including weapon and ability damage. Requires cheats. |
| citadel_enable_no_hero_death |  |  | Enables invincibility (your health will never go below 1). Requires cheats. |
| citadel_disable_no_hero_death |  |  | Disables invincibility. Requires cheats. |
| citadel_display_new_player_recommendations | true/false | true | Turns the "Great for New Players" banner on/off when selecting a hero. |
| citadel_hero_testing_enabled | true/false | false | Enables the "Testing Tools" menu from the Hero Sandbox. Enabling the menu does not require cheats, but using any of this menu's functionality will. |
| citadel_hero_testing_infinite_money | true/false | false | Gives players infinite souls and ability points. |
| citadel_hud_visible | true/false | true | Shows/hides the HUD. |
| citadel_pause |  |  | Pause the match. |
| citadel_player_move_speed_scale | number | 1.0 | Scales movement speed causing players to move faster or slower. Requires cheats. |
| citadel_pregame_duration | number | 10.0 | Changes the duration of the pregame (countdown before the game starts). |
| citadel_region_override | - -1: Auto - 0: North America - 1: Europe - 2: Asia - 3: South America - 4: Europe (not sure if this is different from 1) - 5: Oceania | -1 | Overrides your matchmaking region. **(Currently does not work)** |
| citadel_show_bullet_lag_compensation | number | 0 | How long to show bullet hitboxes. Green hitbox is client, red hitbox is server. |
| citadel_solo_bot_match | true/false | false | Gets enabled by bot match configs. When disabled, bots don't move. This also enables the pregame countdown.   Not sure what else it does. |
| citadel_create_unit | Hero name from dump_hero_names |  | Spawns an allied dummy bot in front of the player. Requires cheats |
| citadel_spawn_nearby_neutrals |  |  | Respawns nearby neutral camps. Requires cheats. |
| citadel_spawn_practice_bots | true/false | false | Enable to spawn bots when the game starts.   You can also set this to true during a game to spawn bots (although setting it to false, kicking bots, and setting it to true again will not respawn bots). |
| citadel_spawn_practice_bots_count | number |  | Number of practice bots to spawn when citadel_spawn_practice_bots is set to true. |
| citadel_test_survey_popup |  |  | Shows the post-match survey popup asking players to rate the match. |
| citadel_unit_status_use_new | true/false |  | Enables experimental health bars. |
| citadel_unlock_flex_slots |  |  | Unlocks all flex slots. Requires cheats. |
| citadel_unpause_countdown | number | 3 | Changes how many seconds the countdown will last when the game is unpaused. Requires cheats. |
| citadel_weapon_damage_multiplier | number | 1.0 | Adds a multiplier to weapon damage output. Does not affect ability damage. Requires cheats. |
| deadlock_early_development_warning_disabled | true/false | false | Disables the Early Development Build popup when the game starts. This gets set to true if you close the popup after checking "Don't show this again". |
| deadlock_get_old_builds |  |  | Downloads and prints out all of the build data for your account prior to the new builds feature.   Added in Update:August 6, 2024. |
| deadlock_post_match_survey_disabled | true/false | false | Disables the post-match survey. This gets set to true if you submit or skip a survey after checking "Don't show this again". |
| disconnect |  |  | Disconnect from the current match. |
| dump_hero_names |  |  | Lists the internal names of all available heros. Requires cheats. |
| healthpct | 0 - 100 |  | Sets your health to the given percentage of your max health. Requires cheats. |
| hud_damagemeter | true/false | false | Displays your current DPS next to your crosshair. Requires cheats. |
| hurtme |  |  | Deals 10 damage to yourself. Requires cheats. |
| killme |  |  | Kills you. |
| kingme |  |  | Gives you 1.2 million souls and levels up all your abilities. Requires cheats. |
| map | - dl_midtown: The main multiplayer map - dl_streets: 4 lanes map - street_test: Old version of 4 lanes map (before Update:September 26, 2024) - new_player_basics: The Hero Sandbox map - 1v1_test: Seems like an early, smaller version of street_test - hero_testing: Seems like an early Hero Sandbox |  | Starts a game and loads into the chosen map.   When used in a multiplayer lobby, this command will kick everyone from the server. Use changelevel to switch maps without kicking everyone. |
| npc_destroy | The name of an NPC to destroy (type npc_destroy<space> to see a list of names).   If no name is provided, destroys the NPC you're looking at. |  | Destroys an NPC (troopers, guardians, walkers, etc.).   As opposed to npc_kill, which causes the standard death sequence, this command zaps the NPC out of existence. |
| npc_kill | The name of an NPC to kill (type npc_kill<space> to see a list of names).   If no name is provided, kills the NPC you're looking at. |  | Kills an NPC (troopers, guardians, walkers, etc.).   This causes the standard death sequence with particles, announcer lines, drops souls, etc. |
| private_lobby_create |  |  | Brings up a menu that allows players to create a private lobby hosted on Valve servers.   Added in Update:September 12, 2024. |
| quit |  |  | Closes the game. |
| resetme |  |  | Resets your level, abilities, and souls. Requires cheats. |
| selecthero | Hero name from dump_hero_names |  | Requires you to be on the hero selection screen, or have citadel_hero_testing_enabled set to true. |
| trooper_kill_all |  |  | Kills all non-neutral creeps and guardians that aren't shielded. Requires cheats. |
| trooper_kill_non_bosses |  |  | Kills all non-neutral creeps. Requires cheats. |

## All Known Convars/Commands

[edit | edit source]

| Command | Default value | Flags | Description |
| --- | --- | --- | --- |
| @panorama_min_comp_layer_cache_cost_TURNED_OFF | ? |  |  |
| _record | cmd | norecord, release | Record a demo incrementally. |
| adsp_debug | 0 | archive |  |
| ai_debug_decisionmaking | false | sv, a | Draw sparks on NPCs in their thinks. Sparks at their feet mean they skipped decision making, sparks high above them means they didn't. |
| ai_debug_dyninteractions | 0 | sv, cheat | Debug the NPC dynamic interaction system. |
| ai_debug_enemy_position | false | sv, cheat | Draw a debug line from a selected NPC to its enemy. |
| ai_debug_los | 0 | sv, cheat | NPC Line-Of-Sight debug mode. If 1, solid entities that block NPC LOC will be highlighted with white bounding boxes. If 2, it'll show non-solid entities that would do it if they were solid. |
| ai_debug_scripted_sequence | false | sv, cheat |  |
| ai_debug_shoot_positions | 0 | sv, cl, rep, cheat |  |
| ai_debug_squadslotusage | false | sv, cheat | Report squad slot usage for npc_selected NPCs. |
| ai_disable | cmd | sv, cheat | Bi-passes all AI logic routines and puts all NPCs into their idle animations.  Can be used to get NPCs out of your way and to test effect of AI logic routines on frame rate |
| ai_disabled | false | sv, cl, rep, cheat |  |
| ai_drop_hint | cmd | sv, cheat | Drop an ai_hint at the player's current eye position. |
| ai_ignore_collision_player_noclip | false | sv, a, cheat |  |
| ai_inhibit_spawners | false | sv, cheat |  |
| ai_keep_interrupt_path_across_schedules | true | sv, cheat |  |
| ai_motor_debug | 0 | sv, cheat |  |
| ai_motor_debug_animgraph | false | sv, cheat |  |
| ai_motor_debug_override_path | false | sv, cheat |  |
| ai_motor_debug_path | false | sv, cheat |  |
| ai_motor_debug_transitions | false | sv, cheat |  |
| ai_motor_draw_entity_facing | false | sv, cheat |  |
| ai_motor_nav_links_force_facing_time | 12 | sv, cheat |  |
| ai_navigator_repath_enable | true | sv, cheat | Enable dynamic repathing based on goal movement. |
| ai_navigator_repath_on_change | true | sv, cheat | When nav mesh changes along an NPC's existing path, force a repath. |
| ai_navigator_repath_tolerance_alpha | 20 | sv, cheat | The distance a target entity can move before triggering a repath is ( arrival time * ai_navigator_repath_tolerance_alpha ), clamped to the min / max allowed values. |
| ai_navigator_repath_tolerance_max | 300 | sv, cheat | The maximum distance that a target entity can move before triggering a repath to that target. |
| ai_navigator_repath_tolerance_min | 8 | sv, cheat | The minimum distance that a target entity can move before triggering a repath to that target. |
| ai_navigator_repath_tolerance_min_speed | 100 | sv, cheat | When calculating repathing tolerance, clamp entity speed to be at least this value (i.e. consider slow entities to be this fast). |
| ai_navigator_snap_to_ground_goal | false | sv, cheat |  |
| ai_navigator_use_arrival_direction | true | sv, cheat |  |
| ai_off_nav_show_nearest | false | sv, cheat |  |
| ai_path_return_a | 0.5 | sv, cheat |  |
| ai_path_return_d | 50 | sv, cheat |  |
| ai_path_return_parallel_speed | 100 | sv, cheat |  |
| ai_path_return_t | 2 | sv, cheat |  |
| ai_path_show_discard_immediately | false | sv, cheat |  |
| ai_report_task_timings_on_limit | false | sv, a |  |
| ai_resume | cmd | sv, cheat | If NPC is stepping through tasks (see ai_step ) will resume normal processing. |
| ai_select_box_alpha | 20 | sv, a | The select box alpha. |
| ai_setenabled | cmd | sv, cheat | Like ai_disable but you manually specify the state (with a 0 or 1) instead of toggling it. |
| ai_show_task_fail | 0 | sv, cheat |  |
| ai_step | cmd | sv, cheat | NPCs will freeze after completing their current task.  To complete the next task, use 'ai_step' again.  To resume processing normally use 'ai_resume' |
| ai_think_limit_label | false | sv, a |  |
| ai_vehicle_avoidance | true | sv, cheat |  |
| alias | cmd | release | Alias a command. |
| anim_resource_validate_on_load | true | release | Validates the animation group channel list against the animations on load for every animation |
| animated_material_attributes | true | cl, cheat |  |
| animevents_dump | cmd | sv, cheat | List all the currently registered anim events. |
| animgraph2testprop_create | cmd | sv, cheat | Create  animgraph2 test prop a short distance in front. |
| animgraph_debug | false | sv, cl, rep, cheat | Debug animation graph |
| animgraph_debug_entindex | 0 | sv, cl, rep, cheat | The entity to specifically debug |
| animgraph_footlock_ik_enable | true | cheat | Enable IK. |
| animgraph_record_all | false | sv, cl, rep, cheat | Automatically start recording AnimGraphs when they get created, and save them to disk when they are destroyed |
| animgraph_set_parameter_bool | cmd | sv, cheat | Specified entities will have the specified bool parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_set_parameter_enum | cmd | sv, cheat | Specified entities will have the specified enum parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_set_parameter_float | cmd | sv, cheat | Specified entities will have the specified float parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_set_parameter_int | cmd | sv, cheat | Specified entities will have the specified int parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_set_parameter_string | cmd | sv, cheat | Specified entities will have the specified bool parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_set_parameter_vector | cmd | sv, cheat | Specified entities will have the specified vector parameter set to the value specified.  Useful for animators to test.  Arguments: <entity> <parameter name> <value you want to send to animgraph for the entity> |
| animgraph_slope_draw_raycasts | false | sv, cl, rep, cheat |  |
| animgraph_slope_enable | false | sv, cl, rep, cheat |  |
| animgraph_trace_static_only | false | sv, cl, rep, cheat |  |
| announce_create | cmd | cl, release | <title> <message> <URL> [Priority] Create a new announcement with the specified title, message, and URL. use empty quotes if you want to skip message or URL |
| announce_delete | cmd | cl, release | <ID> Deletes the specified announcement ID |
| announce_show_ids | false | cl, release | When set, will show the IDs of the various announcements, making updating/deleting easier |
| announce_update | cmd | cl, release | <ID> <title> <message> <URL> [Priority] Create a new announcement with the specified title, message, and URL. use empty quotes if you want to skip message or URL |
| audio_display_soundstack_debug_base_3d | false | sv, cheat | Displays citadel_base_3d sound stack debug. |
| audio_display_soundstack_debug_dialog | false | sv, cheat | Displays citadel_dialog sound stack debug. |
| audio_log_damage_recency_bias | false | sv, cheat | Prints player damage recency information. |
| automatically_open_saved_animgraph_recording | false | sv, cl, a, user, rep |  |
| axis | cmd | sv, cheat | Draw an axis  Arguments:   x y z pitch yaw roll <lifetime = 10.0> <r g b a> |
| ban_ignore_after_player_abandons | 1 | sv, cheat | After this many players have abandoned a match, no longer penalize additional abandons for the match. Set to 0 to not penalize abandoners |
| battery_saver | false | archive | OBSOLETE replaced by mobile_fps_* - Battery saver mode. 0=off, 1=on |
| benchframe | cmd | release | Takes a snapshot of a particular frame in a time demo. |
| bind | cmd | release | Bind a key. |
| binddefaults | cmd | release | Bind all keys to their default values. |
| bindss | cmd | release | Bind a key for a particular splitscreen player. |
| bot_kick_all | cmd | sv, cheat | Kick all the bots |
| bot_mimic | 0 | sv, cl, rep, cheat, release | Allows bots to mimic player |
| bot_mimic_spec_buttons | true | cl, cheat | +attack, +jump etc are used for spectator control instead of being passed on to spectated bot |
| bot_mimic_target | cmd | sv, cheat | Selects the targeted bot for mimicking |
| bot_mimic_yaw_offset | 180 | sv, cheat | Offsets the bot yaw. |
| bot_puppet | 0 | sv, cl, rep, cheat, release | Allows bots to be puppeteered by the player.  The player will do nothing while the bots perform the inputs |
| bot_puppet_target | cmd | sv, cheat | Selects the targeted bot for puppeteering |
| bot_record_target | cmd | sv, cheat | Selects the targeted bot for puppeteering |
| box | cmd | sv, cheat | Draw a bbox  Arguments:  minx miny miny maxx maxy maxz <lifetime = 10.0> <r g b a> |
| buddha | false | sv, nf, cheat | Player takes damage but won't die |
| buddha_ignore_bots | false | sv, nf, cheat | Bots always buddha 0 |
| buddha_reset_hp | 1 | sv, nf, cheat | HP to set when damaged below zero in Buddha Mode |
| bug_submitter_override | 0 | archive |  |
| button_info | cmd | release | Display information about the specified key or button. |
| c_maxdistance | 200 | cl, archive |  |
| c_maxpitch | 90 | cl, archive |  |
| c_maxyaw | 135 | cl, archive |  |
| c_mindistance | 30 | cl, archive |  |
| c_minpitch | 0 | cl, archive |  |
| c_minyaw | -135 | cl, archive |  |
| c_orthoheight | 100 | cl, archive |  |
| c_orthowidth | 100 | cl, archive |  |
| c_thirdpersonshoulder | false | cl, archive |  |
| c_thirdpersonshoulderaimdist | 120 | cl, archive |  |
| c_thirdpersonshoulderdist | 40 | cl, archive |  |
| c_thirdpersonshoulderheight | 5 | cl, archive |  |
| c_thirdpersonshoulderoffset | 20 | cl, archive |  |
| cam_collision | 1 | cl, archive | When in thirdperson and cam_collision is set to 1, an attempt is made to keep the camera from passing though walls. |
| cam_command | cmd | cl, cheat | Tells camera to change modes |
| cam_idealdelta | 4 | cl, archive | Controls the speed when matching offset to ideal angles in thirdperson view |
| cam_idealdist | 150 | cl, archive |  |
| cam_ideallag | 4 | cl, archive | Amount of lag used when matching offset to ideal angles in thirdperson view |
| cam_idealpitch | 0 | cl, archive |  |
| cam_idealyaw | 0 | cl, archive |  |
| cam_showangles | false | cl, cheat | When in thirdperson, print viewangles/idealangles/cameraoffsets to the console. |
| cam_snapto | false | cl, archive |  |
| camortho | cmd | cl, cheat | Switch to orthographic camera. |
| cast_aabb | cmd | sv, cheat | Tests box collision detection |
| cast_capsule | cmd | sv, cheat | Tests capsule collision detection |
| cast_convex | cmd | sv, cheat | Tests convex hull collision detection |
| cast_cylinder | cmd | sv, cheat | Tests cylinder collision detection |
| cast_intervals | cmd | sv, cheat | Tests interval ray cast |
| cast_obb | cmd | sv, cheat | Tests cylinder collision detection |
| cast_physics | cmd | sv, cheat | Tests physics shape collision detection |
| cast_ray | cmd | sv, cheat | Tests ray cast |
| cast_sphere | cmd | sv, cheat | Tests sphere cast |
| cc_delay_time | 0.25 | cl, archive | Close caption delay before showing caption. |
| cc_lang | 0 | cl, archive | Current close caption language (emtpy = use game UI language) |
| cc_linger_time | 1 | cl, archive | Close caption linger time. |
| cc_spectator_only | false | cl, archive |  |
| cc_subtitles | false | cl, archive | If set, don't show sound effect captions, just voice overs (i.e., won't help hearing impaired players). |
| cc_vr_caption_speed | 1 | cl, archive | 0 = slow, 1 = medium (default), 2 = fast |
| cc_vr_font_size | 1 | cl, archive | 0 = small, 1 = med (default), 2 = large |
| cc_vr_width | 1 | cl, archive | 0 = narrow, 1 = med (default), 2 = wide |
| changelevel | cmd | release | changelevel <mapname> : Multiplayer change level. |
| +chatwheel | cmd | cl, release | Opens chatwheel menu while held |
| +chatwheel_pingwheel | cmd | cl, release | Opens the second chatwheel menu while held |
| citadel_1v1_bonus_health | 0 | sv, cl, rep, cheat |  |
| citadel_1v1_bonus_health_regen | 0 | sv, cl, rep, cheat |  |
| citadel_1v1_bonus_tech_power | 0 | sv, cl, rep, cheat |  |
| citadel_1v1_bonus_weapon_power | 0 | sv, cl, rep, cheat |  |
| citadel_1v1_bullet_damage_multiplier | 1 | sv, cl, rep, cheat |  |
| citadel_1v1_tech_damage_multiplier | 1 | sv, cl, rep, cheat |  |
| citadel_ability_cooldown_max | 0 | sv, cl, rep, cheat |  |
| citadel_ability_debug | false | sv, cl, rep, cheat |  |
| citadel_ability_preview_path_debug_draw_dt | 0.075 | cl, archive | DT for debug drawing ability preview path. |
| citadel_ability_target_debug | 0 | sv, cl, rep, cheat |  |
| citadel_activate_cps_for_team | cmd | sv, cheat | Makes the CPs for a team available to capture |
| citadel_activate_window_on_unpause | false | cl, release | If set, brings Citadel to the foreground when unpaused |
| citadel_active_lane | 0 | sv, cl, rep, release | Which lane should be active? 0 means all |
| citadel_air_drag_min | 0.2 | sv, cl, rep, cheat |  |
| citadel_aircontrol_speed | 50 | sv, cl, rep, cheat |  |
| citadel_allow_client_higher_version_for_reconnect | true | cl, release | When set to true, the client is allowed to connect so long as the client compat version is higher than the server's |
| citadel_allow_duplicate_heroes | false | sv, cl, rep, release | If enabled, heroes can be selected by multiple players |
| citadel_allow_purchasing_anywhere | false | sv, cl, rep, cheat | If enabled, you can purchase upgrades anywhere |
| citadel_allow_ranked_schedule_selection | false | cl, release |  |
| citadel_assume_pawn_control | cmd | sv, cheat | Take control of the pawn under the crosshair, or by name if specified |
| citadel_ban_account | cmd | cl, release | 1> <Ban HWID: 0|1> Bans the specified account |
| citadel_book_open | cmd | cl, release | [BookID/Book Name] Opens up the specified book by ID or name |
| citadel_boss_tier_3_testing_enter_phase2 | false | sv, cheat |  |
| citadel_boss_tier_3_testing_reset | cmd | sv, cheat | Respawns the boss |
| citadel_bot_ability_friendly_life_threshold | 70 | sv, rep, release | Maximum life for friendly ability to be used (prevents healing when full health) |
| citadel_bot_ability_friendly_pitch | 60 | sv, rep, release | Pitch (aiming down) for bots when using a friendly ability |
| citadel_bot_ability_min_cast_range | 800 | sv, rep, release | Default Cast Range for abilities that don't specify |
| citadel_bot_ability_min_cast_range_friendly | 800 | sv, rep, release | Default Enemy range to use friendly abilities |
| citadel_bot_ability_window_size | 0.85 | sv, rep, release | How much in range before doing an ability (ie not casting on edges) |
| citadel_bot_attack_enemies_inaccuracy | 0 | sv, rep, release | Bots choose a random angle in this range to offset their perfect aim |
| citadel_bot_attack_enemies_inaccuracy_distance | 25 | sv, rep, release | Distance (m) to make bots even worse accuracy |
| citadel_bot_attack_enemies_inaccuracy_distance_scale | 1.5 | sv, rep, release | Scale the accuracy by this amount at distance |
| citadel_bot_attack_enemies_inaccuracy_scale | 1 | sv, rep, release | When trying to miss, how much to scale each miss attempt |
| citadel_bot_attack_enemies_inaccuracy_threat_scale | 0.5 | sv, rep, release | Scale inaccuracy by this amount when threatened |
| citadel_bot_attack_miss_chance | 0 | sv, rep, release | Desired bot miss chance, [0.0 - 1.0] |
| citadel_bot_attempt_deny_orb_pct | 10 | sv, rep, release | Percentage of the time to look for red orbs to shoot |
| citadel_bot_attempt_orb_range | 35 | sv, rep, release | Range(m) to Scan for Orbs |
| citadel_bot_attempt_orb_start_time | 180 | sv, rep, release | Try to deny orbs |
| citadel_bot_attempt_secure_orb_pct | 5 | sv, rep, release | Percentage of the time to look for gold orbs to shoot |
| citadel_bot_avoid_human_ally | false | sv, rep, release | Forces citadel bots to avoid human allies |
| citadel_bot_bonus_regen | 0 | sv, rep, release |  |
| citadel_bot_bonus_regen_outofsight | 0.03 | sv, rep, release |  |
| citadel_bot_bonus_run_speed | 6 | sv, rep, release |  |
| citadel_bot_brain_aim_angle_attack | 0.9 | sv, rep, release | Min Dot Product result from target that we will try to shoot from |
| citadel_bot_brain_aim_inaccuracy | 0 | sv, rep, release | Max Angle for Inaccuracy |
| citadel_bot_brain_aim_inaccuracy_speed | 0.01 | sv, rep, release | How fast the inaccuracy moves - mimic mouse movement correction |
| citadel_bot_brain_aim_vertical_offset | 0 | sv, rep, release | How many vertical units to aim from world space center on players / troopers |
| citadel_bot_brain_enemy_reaction_time | 0.75 | sv, rep, release | Amount of time for a bot to react to a player |
| citadel_bot_brain_infrequent_tick_rate | 60 | sv, rep, release |  |
| citadel_bot_brain_melee_chance | 0.1 | sv, rep, release |  |
| citadel_bot_brain_melee_chance_in_reload | 0.3 | sv, rep, release |  |
| citadel_bot_brain_melee_check_time | 30 | sv, rep, release |  |
| citadel_bot_brain_melee_heavy_chance | 0.5 | sv, rep, release |  |
| citadel_bot_brain_melee_heavy_hold_time | 0.31 | sv, rep, release |  |
| citadel_bot_brain_move_goal_tolerance | 40 | sv, rep, release | How close to goal to count as made it |
| citadel_bot_brain_parry_chance | 0.02 | sv, rep, release |  |
| citadel_bot_brain_stop_shotting_los_time | 0.5 | sv, rep, release | Amount of time for no Los to stop shooting at enemy |
| citadel_bot_brain_zipline_distance | 400 | sv, rep, release | Distance away from zipline node we want for pathing to it |
| citadel_bot_buddy | 0 | sv, cl, rep, release | List of heroes to choose from that should follow a player around |
| citadel_bot_choose_balanced_lanes | true | sv, rep, release | Bots try to balance lanes |
| citadel_bot_choose_lane_on_death | false | sv, rep, release | Bots pick a new lane when they die |
| citadel_bot_choose_lane_on_interval | 5 | sv, rep, release | Bots pick on a time interval |
| citadel_bot_critical_health | 0.15 | sv, rep, release | Critical |
| citadel_bot_critical_health_pushed | 0.35 | sv, rep, release | Critcal at tower |
| citadel_bot_crouch | false | sv, rep, release | Forces citadel bots to crouch |
| citadel_bot_enemy_hero_engage_distance | 10 | sv, rep, release | Distance away from target to search for an attack location |
| citadel_bot_engage_distance | 1500 | sv, rep, release | Distance citadel bots are willing to engage enemies at |
| citadel_bot_engage_hero_distance | 0 | sv, rep, release | Extra distance citadel bots are willing to engage heroes at |
| citadel_bot_engage_lane_side_dist | 200 | sv, rep, release | Distance citadel bots will engage to the left or right of the target |
| citadel_bot_engage_player_side_dist | 200 | sv, rep, release | Distance citadel bots will engage to the left or right of the target |
| citadel_bot_fight_for_idol | false | sv, rep, release | Fight for the idol |
| citadel_bot_fight_midboss | false | sv, rep, release | Fight the midboss (Note: this doesn't seem to work in the latest update.) |
| citadel_bot_free_gold_per_minute | 0 | sv, rep, release | Bots get free gold over time |
| citadel_bot_free_gold_per_minute_scaled | 0 | sv, rep, release | GPM that scales with game time |
| citadel_bot_give_team_gold | cmd | sv, cheat | Give all bots on a particular team gold |
| citadel_bot_hero_testing_pitch | 5 | sv, rep, release | Aim Pitch in Hero Testing |
| citadel_bot_jump | false | sv, rep, release | Forces citadel bots to jump |
| citadel_bot_jump_sometimes | true | sv, rep, release | Forces citadel bots to attack nearby enemies |
| citadel_bot_lane_change_duration | 5 | sv, rep, release | Duration Bot prioritizes changing lanes vs fighting |
| citadel_bot_last_hit_distance | 0 | sv, rep, release | Extra distance citadel bots are willing to engage enemies at to get last hits |
| citadel_bot_last_hit_threshold | 0 | sv, rep, release | Forces citadel bots to prioritize getting last hits on enemies below this health |
| citadel_bot_list_ents | cmd | sv, cheat | List ent id of all players that are bots in this game |
| citadel_bot_list_objectives_ent | cmd | sv, cheat | List all entities that are associated with a Citadel Game Objective |
| citadel_bot_low_health | 0.3 | sv, rep, release | Low Health |
| citadel_bot_low_health_pushed | 0.5 | sv, rep, release | When pushed against tower |
| citadel_bot_max_attacker_memory | 6 | sv, rep, release | How long to remember recent attackers |
| citadel_bot_melee | 0 | sv, rep, release | Forces citadel bots to melee continuously, 1: light, 2: Heavy |
| citadel_bot_message_interval | 20 | sv, rep, release | Min time between messages a player bot can send |
| citadel_bot_mimic_player_pitch | true | sv, rep, release | User player's pitch in hero testing |
| citadel_bot_move_random | false | sv, rep, release | Forces citadel bots to move all around |
| citadel_bot_playrecording | cmd | sv, cheat | Play back commands recorded via 'citadel_bot_record' |
| citadel_bot_practice_opponent | hero_gigawatt | sv, rep, release |  |
| citadel_bot_practice_teammate | hero_kelvin | sv, rep, release |  |
| citadel_bot_projectile_range_scale | 0.5 | sv, rep, release | Factor from Projectile speed to usable range |
| citadel_bot_purchase_random_upgrades | 0 | sv, rep, release | Citadel bots will randomly purchase available upgrades every few seconds |
| citadel_bot_purchase_upgrades_in_order | 0 | sv, rep, release | Citadel bots will purchase available upgrades in order every few seconds |
| citadel_bot_record | 0 | sv, rep, release | Causes bots to mimic your commands as well as record them to be replayed |
| citadel_bot_reload_pct | 0 | sv, rep, release | Bot reloads when clip is this low |
| citadel_bot_roll_after_damage | true | sv, rep, release | Forces citadel bots to attack nearby enemies |
| citadel_bot_roll_chance | 0.4 | sv, rep, release | How often bots will roll given damage conditions |
| citadel_bot_roll_chance_lowhealth_scale | 1.6 | sv, rep, release |  |
| citadel_bot_roll_frequency | 2 | sv, rep, release | Time between roll attempts |
| citadel_bot_sensing_tick_interval | 12 | sv, rep, release | How many ticks between the bot performing sensing |
| citadel_bot_shoot | 0 | sv, rep, release | Forces citadel bots to fire continuously. 1:scope shooting, 2:unscope shooting. |
| citadel_bot_shoot_duration | 0.75 | sv, rep, release | Seconds after a bot sees you before it can react |
| citadel_bot_spend_random_ap | 0 | sv, rep, release |  |
| citadel_bot_takeover_ally_range | 30 | sv, rep, release | How far from Allies that is acceptable |
| citadel_bot_takeover_spend_currency_time | 240 | sv, rep, release | How much time until a takeover bot till spend gold/ap |
| citadel_bot_takeover_time | 30 | sv, rep, release | Time for a disconnected player to be taken over by a bot |
| citadel_bot_test_mode | false | sv, rep, release | Set citadel bots to be and in test mode (default idle) |
| citadel_bot_use_ability | 0 | sv, rep, release | Causes Bot to Constantly use Ability when its available |
| citadel_bot_use_ability_cooldown | 5 | sv, rep, release | Time between bot using ability |
| citadel_bot_use_ability_once | false | sv, rep, release | Set if you only want enemy to use ability once and stop |
| citadel_bot_use_item_ability | 0 | sv, rep, release | Causes Bot to Constantly use Ability when its available |
| citadel_bot_visual_reaction_time | 0.75 | sv, rep, release | Seconds after a bot sees you before it can react |
| citadel_bot_zig_zag | 0 | sv, rep, release | Forces citadel bots to zig-zag side to side if > 0 or back and forth if < 0 |
| citadel_bounty_aoe_radius | 750 | sv, cl, rep, cheat | The radius in which teammates gain a portion of bounties |
| citadel_bounty_aoe_radius_neutrals | 800 | sv, cl, rep, cheat | The radius in which teammates gain a portion of Neutral |
| citadel_bounty_aoe_radius_troopers | 1968.5 | sv, cl, rep, cheat | The radius in which teammates gain a portion of things besides Neutrals and Players |
| citadel_bounty_aoe_radius_troopers_from_hero | 1378 | sv, cl, rep, cheat | The radius in which teammates gain a portion of things besides Neutrals and Players |
| citadel_bullet_obscured_shot_distance | 256 | sv, cl, rep, cheat |  |
| citadel_camera_height | 63 | cl, cheat | The look at point of the camera is vertically offset by this distance. |
| citadel_camera_height_approach_speed | 100 | cl, cheat |  |
| citadel_camera_height_npc | 33 | cl, cheat | The look at point of the camera is vertically offset by this distance when viewing NPC units. |
| citadel_camera_interior_medium_distance | 75 | cl, cheat | How car back the camera is allowed to go in interior spaces |
| citadel_camera_interior_small_distance | 25 | cl, cheat | How car back the camera is allowed to go in interior spaces |
| citadel_camera_offset | -25 | cl, cheat | The look at point of the camera is horizontally offset by this distance. |
| citadel_camera_pitch_inverted | false | cl, archive | Set to 1 to have inverted mouse pitch |
| citadel_camera_sensitivity | 1 | cl, archive | Mouse sensitivity for the camera |
| citadel_complete_new_player | cmd | cl, release | [flag] Marks the new player state as complete |
| citadel_coop_sandbox | false | sv, cl, rep, release |  |
| citadel_crate_client_notification_time | 30 | sv, cheat |  |
| citadel_crate_delivery_base_payoff | 0 | sv, cheat |  |
| citadel_crate_delivery_overtime_bonus | 50 | sv, cheat |  |
| citadel_crate_disable_early_spawn | true | sv, cheat |  |
| citadel_crate_early_spawn_delay | 30 | sv, cheat |  |
| citadel_crate_respawn_interval | 300 | sv, cheat |  |
| citadel_crate_spawn_initial_delay | 600 | sv, cheat |  |
| citadel_create_test_time_warp | cmd | sv, cheat | Create a time warp volume at your feet |
| citadel_create_unit | cmd | sv, vconsole_fuzzy | none] [team] - Creates an unit.  Pass 'my_hero' as hero_name to use your current hero |
| citadel_crosshair_color_b | 255 | cl, archive |  |
| citadel_crosshair_color_g | 255 | cl, archive |  |
| citadel_crosshair_color_r | 255 | cl, archive |  |
| citadel_crosshair_dot_opacity | 0.7 | cl, archive |  |
| citadel_crosshair_dot_outline_opacity | 0.9 | cl, archive |  |
| citadel_crosshair_hit_marker_duration | 0.1 | cl, archive |  |
| citadel_crosshair_pip_border | true | cl, archive |  |
| citadel_crosshair_pip_gap | 3 | cl, archive |  |
| citadel_crosshair_pip_height | 16 | cl, archive |  |
| citadel_crosshair_pip_opacity | 0.4 | cl, archive |  |
| citadel_crosshair_pip_width | 4 | cl, archive |  |
| citadel_damage_text_batching_window_ability | 1.05 | cl, archive | When ability damage events are within this amount of time of each other, they will be added together into a single entry. |
| citadel_damage_text_batching_window_bullet | 1.05 | cl, archive | When bullet damage events are within this amount of time of each other, they will be added together into a single entry. |
| citadel_damage_text_distance_far | 4000 | cl, archive | Far distances at which we use far offsets for damage numbers |
| citadel_damage_text_distance_near | 100 | cl, archive | Near distance at which we use the near offsets for damage numbers |
| citadel_damage_text_height_offset_far | 200 | cl, archive | How much to offset damage numbers above when far from the camera |
| citadel_damage_text_height_offset_near | 130 | cl, archive | How much to offset damage numbers above when near from the camera |
| citadel_damage_text_lifetime | 1.5 | cl, archive | How long do numbers live. |
| citadel_damage_text_x_offset_far | 0 | cl, archive | How much to offset damage numbers left and right when far from the camera |
| citadel_damage_text_x_offset_near | 0 | cl, archive | How much to offset damage numbers left and right when near the camera |
| citadel_death_replay_enabled | true | sv, cl, rep, release |  |
| citadel_debug_ent_los | false | sv, cl, rep, cheat | Debug:  Draw Spheres on Ent Being Los Tested |
| citadel_decrease_replay_speed | cmd | cl, release | Decrease the Replay speed while watching a replay |
| citadel_deny_text_height_offset | 35 | cl, archive | How much higher should deny text show up. |
| citadel_deny_text_max_distance | 4000 | cl, archive | How far away before we stop showing in world deny events. |
| citadel_disable_duplicate_heroes | cmd | sv, cheat, release | Disable usage of Duplicate Heroes |
| citadel_disable_fast_cooldowns | cmd | sv, cheat | Disable fast cooldowns |
| citadel_disable_fast_stamina | cmd | sv, cheat | Disable fast stamina |
| citadel_disable_no_hero_death | cmd | sv, cheat | Make heroes able to die |
| citadel_disable_unlimited_ammo | cmd | sv, cheat | Disable unlimited ammo |
| citadel_display_new_player_recommendations | true | cl, release | Do we want to show the decorations for new player friendly heroes? |
| citadel_dps_multiplier | 1 | sv, cl, rep, cheat | Increase weapon damage for testing |
| citadel_enable_duplicate_heroes | cmd | sv, cheat, release | Enable usage of Duplicate Heroes |
| citadel_enable_fast_cooldowns | cmd | sv, cheat | Enables fast cooldowns |
| citadel_enable_fast_stamina | cmd | sv, cheat | Enables fast stamina |
| citadel_enable_no_hero_death | cmd | sv, cheat | Make heroes unable to die |
| citadel_enable_unlimited_ammo | cmd | sv, cheat | Enables unlimited ammo |
| citadel_fake_bots_as_pinging_player | false | sv, cheat |  |
| citadel_fake_number_of_games_played | -1 | cl, release |  |
| citadel_fake_number_of_ranked_games | -1 | cl, release | Fake the number of ranked games you've played. -1 is disabled |
| citadel_fake_ranked_open_status | -1 | cl, release | Fake a ranked mode status. -1 is disabled, 0 is fake rank closed, 1 is fake ranked open |
| citadel_fake_schedule_selected | -1 | cl, release |  |
| citadel_fibonacci_sphere_trace | cmd | sv, cheat | Draws the LOS check generated by our fibonacci sphere trace algorithm |
| citadel_fly_accelerate | 2 | sv, cl, rep, cheat |  |
| citadel_forced_hero_model | 0 | sv, cheat | Forces all heroes to use this model |
| citadel_give_gold | cmd | sv, cheat | <gold> Give gold value to all players |
| citadel_give_player_gold | cmd | sv, cheat | <player name> <gold> Gives the specified player gold |
| citadel_gold_text_height_offset | 35 | cl, archive | How much higher should gold text show up. |
| citadel_guide_bot_neutral_info | false | sv, rep, release | Guide bot talks about neutrals |
| citadel_guided_bot_match | false | sv, cl, rep, release |  |
| citadel_guided_bot_match_hint_time_mult | 0.25 | cl, release | How much faster/slower to show hints in guided bot match mode |
| citadel_guided_bot_t1_boss_ignore_damage_threshold | 0 | sv, rep, release |  |
| citadel_gun_max_spread_penalty | 5 | sv, cl, rep, cheat | Max spread penalty you can incur from taking damage |
| citadel_healthbars_enabled | true | cl, release |  |
| citadel_hero_builds_show_all_languages | true | cl, archive release | Whether to show builds from all languages or just your current locale |
| citadel_hero_demo_enable_fast_stamina | false | sv, cl, a, rep, release | Do we enable fast stamina cooldowns |
| citadel_hero_demo_enable_unlimited_ammo | false | sv, cl, a, rep, release | Do we enable unlimited ammo |
| citadel_hero_demo_hero_spawn | hero_inferno | sv, cl, a, rep, release | Which hero do we spawn when we spawn and enemy or ally hero |
| citadel_hero_demo_infinite_resources | true | sv, cl, a, rep, release | Do we start our hero demo with infinite resources |
| citadel_hero_demo_no_cooldowns | false | sv, cl, a, rep, release | Do we start withough cooldowns when launching the hero demo map |
| citadel_hero_demo_no_death | false | sv, cl, a, rep, release | Do we start withough death when launching the hero demo map |
| citadel_hero_demo_no_troopers | false | sv, cl, a, rep, release | Do we start withough troopers when launching the hero demo map |
| citadel_hero_demo_persist_convars | false | sv, cl, a, rep, release | Do we persist convars between sessions in hero demo |
| citadel_hero_demo_spawn_items | 0 | sv, cl, rep, cheat, release | Items to give a hero post spawn |
| citadel_hero_demo_unlock_flex_slots | false | sv, cl, a, rep, release | Do we start flex slots unlocked |
| citadel_hero_roster | 0 | cl, archive release | A comma separated list of hero IDs that hold the currently selected roster heroes |
| citadel_hero_roster_high_priority | 0 | cl, archive release | A comma separated list of hero IDs that hold the currently high priority roster heroes |
| citadel_hero_roster_preferred | 0 | cl, archive release | A comma separated list of hero IDs that hold the currently preferred roster heroes |
| citadel_hero_testing_ability1_state | 0 | sv, cl, rep, release |  |
| citadel_hero_testing_ability2_state | 0 | sv, cl, rep, release |  |
| citadel_hero_testing_ability3_state | 0 | sv, cl, rep, release |  |
| citadel_hero_testing_ability4_state | 0 | sv, cl, rep, release |  |
| citadel_hero_testing_ability_learn_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_ability_purchased_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_ability_upgrade_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_dash_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_dummy_target | 55 | sv, release | Dummy Target heroID |
| citadel_hero_testing_enabled | false | sv, cl, rep, release |  |
| citadel_hero_testing_give_abilities | true | sv, rep, release | Grant Abilities on Character Spawn |
| citadel_hero_testing_guided_sandbox | false | sv, cl, rep, release |  |
| citadel_hero_testing_hide_mods | false | sv, cl, rep, release |  |
| citadel_hero_testing_infinite_money | false | sv, cl, rep, release | Enable infinite money in Hero Testing |
| citadel_hero_testing_jump_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_mantle_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_mods_purchased_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_money | 4000 | sv, rep, release | How much money to buffer item purchases in Hero Testing |
| citadel_hero_testing_movement_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_reload_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_shoot_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_show_intro_modal | false | sv, cl, rep, release |  |
| citadel_hero_testing_show_outro_modal | false | sv, cl, rep, release |  |
| citadel_hero_testing_wasd_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_zipline_attach_finished | false | sv, cl, rep, release |  |
| citadel_hero_testing_zoom_finished | false | sv, cl, rep, release |  |
| citadel_hide_replay_hud | false | cl, release |  |
| citadel_hint_system_disable | false | cl, release | Set to disable hints |
| citadel_hud_exclusive_visible_id | 0 | cl, cheat | When set, only show the panel with the corresponding id |
| citadel_hud_visible | true | cl, release | Turns on/off rendering the HUD |
| citadel_increase_replay_speed | cmd | cl, release | Increase the Replay speed while watching a replay |
| citadel_invert_ping_type | false | cl, archive | Inverts the ping types so single ping would be aggressive and double ping would be passive |
| citadel_item_early_gold_duration | 30 | sv, cheat |  |
| citadel_item_purchases_force_enhanced | false | cl, cheat | Causes any items purchased of given with the give command to be their enhanced versions. |
| citadel_item_glow_local_dist | 800 | cl, cheat |  |
| citadel_item_idol_label_offset | 50 | cl, cheat |  |
| citadel_item_neutral_gold_label_offset | 6 | cl, cheat |  |
| citadel_item_pickup_fall_tolerance | 16 | sv, cheat |  |
| citadel_item_pickup_fallrate | 5 | sv, cheat |  |
| citadel_item_rejuvenator_label_offset | 75 | cl, cheat |  |
| citadel_item_used_text_height_offset | 25 | cl, archive | How much higher item used text show up. |
| citadel_lane_matchups_mmr_variance | 0 | sv, release | specifies how much of a gap between MMR's we allow to randomize lane assignment |
| citadel_last_used_hero_builds | 0 | cl, archive release |  |
| citadel_lock_flex_slots | cmd | sv, cheat | <team number> - Lock the flex slots for a team (or both teams if you omit the team number) |
| citadel_mantle_max_height | 134 | sv, cl, rep, cheat | How high the maximum mantle is |
| citadel_match_details | cmd | cl, release | <MatchID> [Metadata Salt] Opens the match details to the specified match |
| citadel_min_accel_speed | 400 | sv, cl, rep, cheat | How fast we accelerate depends on our move speed - this lower bound ensures it doesn't go below ground friction |
| citadel_minimap_draw_fow | false | cl, cheat |  |
| citadel_minimap_spectator_fow_team_view | 1 | cl, release | Which team to view the minimap as when freeflying |
| citadel_move_goal_tolerance | 8 | sv, cheat | Some extra tolerance for considering an NPC moved to a goal; can be reduced as we fix other issues |
| citadel_new_player_flow_visible | true | cl, archive release | Are we still showing the new player instructions |
| citadel_new_player_progress | 0 | cl, archive release | Tracks the local settings for the new player progress so they can be synchronized with the GC for client authoratative progress |
| citadel_npc_allow_jump_down | true | sv, rep, cheat | Allow NPCs to follow any drop-down navigation links. |
| citadel_npc_health_regen_stall_time | 0 | sv, cheat | How long after the npc gets hit before health regen resumes |
| citadel_observer_roaming_speed | 600 | cl, archive |  |
| citadel_one_on_one_match | false | sv, cl, rep, release |  |
| citadel_one_on_one_match_starting_gold | 0 | sv, cl, rep, cheat, release |  |
| citadel_open_ability_vdata_by_name | cmd | cl, cheat | Open an ability by name in the VData editor |
| citadel_open_ability_vdata_by_slot | cmd | cl, cheat | Open an ability by slot in the VData editor |
| citadel_open_hero_sheet | cmd | cl, release | Open the current hero character sheet |
| citadel_open_hero_vdata_by_name | cmd | cl, cheat | Open the VData editor to a specified hero |
| citadel_open_modeldoc_to_model | cmd | cl, cheat | Open ModelDoc to the model under the cursor.  Pass any parameter to open your own model |
| citadel_open_vdata_file_to_node | cmd | cl, cheat | Open the VData editor to a specified file and node |
| citadel_party_invite_in_game | true | cl, release | When set, only users in game can be invited |
| citadel_pause | cmd | cl, release | Send a game pause request. |
| citadel_pause_countdown | 0 | sv, cheat | Countdown timer to pause after a user has pressed pause |
| citadel_pause_minimum_time | 2 | sv, cheat | Disables unpausing for this many seconds after a pause occurs |
| citadel_per_unit_hotkeys_checked | false | cl, archive |  |
| citadel_player_attack_enemy_npc_fow_reveal_duration | 2 | sv, cheat | How long a player is visible to enemy FOW after attacking an enemy trooper or boss |
| citadel_player_attack_enemy_player_fow_reveal_duration | 1 | sv, cheat | How long a player is visible to enemy FOW after attacking an enemy player |
| citadel_player_glow_begin_delay | 1 | cl, cheat | Enemy players who are visibly obstructed won't glow until they've been revealed via FOW for this long |
| citadel_player_ground_dash_max_percent | 2 | sv, cl, rep, cheat | Max ground dash scale |
| citadel_player_ground_dash_min_percent | 0.6 | sv, cl, rep, cheat | Min ground dash scale |
| citadel_player_move_speed_min | 80 | sv, cl, rep, cheat | Min walk speed |
| citadel_player_move_speed_scale | 1 | sv, cl, rep, cheat | Scales how fast players can move |
| citadel_player_pawn_ag2_enable | false | sv, cl, rep, release |  |
| citadel_player_ping_duration | 6 | sv, cheat |  |
| citadel_player_regen_zone_bonus_base | 60 | sv, cl, rep, cheat | When standing in a regen zone, how much extra do we regen per second? |
| citadel_player_regen_zone_bonus_pct | 6 | sv, cl, rep, cheat | When standing in a regen zone, how much extra do we regen per second based on max health percentage? |
| citadel_pregame_duration | 10 | sv, cheat | How long pre-match is until we start the match |
| citadel_previous_umuted_audio_level | 1 | cl, archive |  |
| citadel_ranked_popup_shown | false | cl, archive | Have we shown the ranked popup for players who are eligible for ranked gameplay. |
| citadel_rapid_stamina_regen | false | sv, cl, rep, cheat |  |
| citadel_record_hero_animgraph | cmd | sv, cheat | Record the animgraph for a specified hero |
| citadel_region_override | -1 | cl, release | Override the region of the client |
| citadel_render_minimap | cmd | cl, release | Render the minimap |
| citadel_replay_manager_download_chunk_size | 1048576 | cl, archive |  |
| citadel_replay_manager_download_simultaneous_requests | 3 | cl, archive |  |
| citadel_replay_toggle_pause | cmd | cl, release | Toggle a replay being paused |
| citadel_reset_new_player | cmd | cl, release | Resets the new player experience back to the initial state |
| citadel_safe_spot_safety_radius | 7 | sv, rep, release | Radius for bots to consider whether a position is safe |
| citadel_safe_spot_samples_max | 3 | sv, rep, release | Maximum number of spots to sample looking for good positioning |
| citadel_safe_spot_samples_min | 1 | sv, rep, release | Minimum number of spots to sample looking for good positioning |
| citadel_safe_spot_target_radius | 6 | sv, rep, release | Radius for bots to look for better locations to path to |
| citadel_send_gc_match_info_s | 30 | sv, cl, rep, release | Determines the rate that we should submit match info up to the GC, 0 disables this functionality |
| citadel_server_all_players_disconnected_grace_period_s | 120 | sv, release | How long a server should run after all players have disconnected before notifying that all players have left |
| citadel_server_max_spectator_slots | 3 | sv, release | The maximum number of spectator slots we allow. This is so that the GC can restrict this remotely if we need to. -1 disables this limit |
| citadel_shop_items_appear_enhanced | false | cl, cheat | Causes items in the shop to visually appear enhanced. Does not cause purcahses to actually be enhanced, however. |
| citadel_show_account_ids | false | cl, release | When set, account IDs will be shown on player tooltips |
| citadel_show_bullet_lag_compensation | 0 | sv, cl, rep, cheat | if > 0.0, show lag compensated hitboxes (value is seconds) whenever a bullet is lag compensated and hits something. |
| citadel_show_npe_bots_modal | true | cl, archive release | Show the NPE Bots modal when navigating to the bots page. |
| citadel_show_npe_modal | true | cl, archive release | Show the NPE modal when navigating to the roster page. |
| citadel_show_post_game_survey | cmd | cl, cheat | Shows post game survey test |
| citadel_solo_bot_match | false | sv, cl, rep, release |  |
| citadel_spawn_all_heroes_in_a_line | cmd | sv, cheat | Spawn all of the heroes as bots in a line in front of you |
| citadel_spawn_nearby_neutrals | cmd | sv, cheat, release | Spawns any neutral camps within 800 units (~20m) |
| citadel_spawn_payload_for_team | cmd | sv, cheat | Spawns a payload for a team |
| citadel_spawn_practice_bots | false | sv, release |  |
| ' citadel_spawn_practice_bots_count | 1 | sv, release |  |
| citadel_spawn_urn | cmd | sv, cheat | Spawn an urn for testing |
| citadel_spectator_voice_mode | true | cl, user | Spectator voice transmit mode: 0 spectators and players, 1 spectators only |
| citadel_spectator_voice_mode_toggle | cmd | cl, release | Toggle the value of citadel_spectator_voice_mode |
| citadel_standing_spread_is_aimed_spread | true | sv, cl, rep, cheat |  |
| citadel_start_lane_challenge | cmd | sv, vconsole_fuzzy | [hero_name] - Creates an unit to lane against in the test map |
| citadel_stop_lane_challenge | cmd | sv, vconsole_fuzzy | Ends the lane challenge |
| citadel_streaming_mode_enabled | false | cl, archive release | Enable to alter various game UI elements |
| citadel_stuck_camera_trace_extra_length | 100 | sv, cl, rep, cheat |  |
| citadel_stuck_normal_find_trace_fallback_elevation | 24 | sv, cl, rep, cheat |  |
| +citadel_swtich_player_cam | cmd | cl, release | Player Cam switching button pressed |
| citadel_teleporter_enabled_time | 480 | sv, cl, rep, cheat |  |
| citadel_test_survey_popup | cmd | cl, cheat | Tests bringing up the survey popup |
| citadel_tether_pull_speed | 200 | sv, cl, rep, cheat |  |
| citadel_tether_pull_speed_scale_per_meter | 120 | sv, cl, rep, cheat |  |
| citadel_tightcamera_alternative | 1.3 | cl, archive | Tight-camera test mode alternative. |
| citadel_time_after_damage_to_show_hints | 10 | cl, release | Time after the local player has taken damage from another player before we show hints again. |
| citadel_toggle_mute | cmd | cl, release | Toggles muting/unmuting the audio. |
| citadel_track_player_vs_player_accuracy | true | sv, cl, rep, cheat |  |
| citadel_trooper_ag2_enable | false | sv, cl, rep, release |  |
| citadel_ui_allow_feature_bot_test | true | cl, release | When true, we can feature bot test matches |
| citadel_ui_prefer_region_spectating | false | cl, release | When true, we will give a boost to spectating matches within our region |
| citadel_ui_watch_active_game_refresh_s | 5 | cl, release | The number of seconds to wait between refreshes of the active matches while on the watch page |
| citadel_unlock_flex_slots | cmd | sv, cheat | <team number> - Unlock the flex slots for a team (or both teams if you omit the team number) |
| citadel_unpause_countdown | 3 | sv, cheat | Countdown duration to the unpause after a user unpauses |
| citadel_update_gc_connection_check_count | 50 | sv, cheat | How many tries we check if the GC is still connected before terminating due to no response |
| citadel_update_gc_connection_check_time | 1200 | sv, cheat | How often the server should check the GC is still connected (in seconds) |
| citadel_update_gc_connection_check_time_variance | 60 | sv, cheat | How much variance to allow the GC check time to avoid swamping the GC (in seconds) |
| citadel_upload_replay_enabled | true | sv, release | Controls if replay uploading is enabled. Mainly used as a kill switch if something goes wrong |
| citadel_use_contextual_ping_wheel_option | true | cl, archive |  |
| citadel_use_ui_keybindings | true | cl, archive release | Use UI key bindings otherwise use engine keybindings. |
| citadel_viewed_book_prototype | false | cl, archive release | Track if they have opened up the book prototype or not yet |
| citadel_viewpunch_damping | 9 | sv, cl, rep, cheat | Bigger number makes the response more damped, smaller is less damped |
| citadel_viewpunch_spring_constant | 15 | sv, cl, rep, cheat | Bigger number increases the speed at which the view corrects |
| citadel_weapon_damage_multiplier | 1 | sv, cl, rep, cheat | Multiply the damage on guns |
| citadel_weapon_normalize_recoil_with_firerate | true | sv, cl, rep, cheat | Keep recoil constant even with fire rate changes. |
| cl_audio_display_soundstack_debug_base_3d | false | cl, cheat | Displays citadel_base_3d sound stack debug. |
| cl_audio_display_soundstack_debug_dialog | false | cl, cheat | Displays citadel_dialog sound stack debug. |
| cl_audio_log_participant_start_messages | false | cl, cheat | Prints when a participant sound message was sent. |
| cl_auto_cursor_scale | true | archive | Automatic cursor size scaling. |
| cl_axis | cmd | cl, cheat | Draw an axis  Arguments:  x y z pitch yaw roll <lifetime = 10.0> <r g b a> |
| cl_box | cmd | cl, cheat | Draw a bbox  Arguments:  minx miny miny maxx maxy maxz <lifetime = 10.0> <r g b a> |
| cl_change_callback_limit | 0.2 | cl, release | change callback msec warning limit |
| cl_checkdeclareclasses | cmd | cheat | Check game code serializers |
| cl_citadel_ability_alt_cast_hold_time | 0.15 | cl, archive user |  |
| cl_citadel_ability_alt_cast_instant_cast_double_tap_timeout | 0.2 | cl, archive user |  |
| cl_citadel_ability_alt_cast_mode | 2 | cl, archive user |  |
| cl_citadel_bebop_beam_draw_points | false | cl, cheat |  |
| cl_citadel_cancel_ability_mode | 1 | cl, archive user |  |
| cl_citadel_items_quickcast_mode | 0 | cl, archive user |  |
| cl_citadel_quickcast_ability1 | 0 | cl, archive user |  |
| cl_citadel_quickcast_ability2 | 0 | cl, archive user |  |
| cl_citadel_quickcast_ability3 | 0 | cl, archive user |  |
| cl_citadel_quickcast_ability4 | 0 | cl, archive user |  |
| cl_citadel_record_hero_animgraph | cmd | cl, cheat | Record the animgraph for a specified hero |
| cl_citadel_selected_hero_build_id | 0 | cl, archive user |  |
| cl_citadel_zoom_is_toggle | false | cl, archive user |  |
| cl_clock_correction | true | cheat | Enable/disable clock correction on the client. |
| cl_clock_recvmargin_spew_interval | 0 | release |  |
| cl_clockdrift_max_ticks | 3 | cheat | Maximum number of ticks the clock is allowed to drift before the client snaps its clock to the server's. |
| cl_connectionretrytime_p2p | 20 | release | Number of seconds over which to spread retry attempts for P2P. |
| cl_cq_min_queue | 0 | user | Used by the client to inform the server of their desired queue length.  Derived from cl_tickpacket_recvmargin_desired and cl_tickpacket_desired_queuelength |
| cl_cursor_scale | 1 | archive | Cursor size scaling factor. |
| cl_debug_overlays_broadcast | false | release | Render debug overlays from server. |
| cl_debugoverlay_cycle_domain | cmd | cl, cheat | Toggles visibility of the debug overlay system. |
| cl_debugoverlay_cycle_state | cmd | cl, cheat | Toggles visibility of the debug overlay system. |
| cl_debugoverlay_dashboard | cmd | cl, cheat | Makes the debug overlay dashboard visible. |
| cl_debugoverlay_hide_imgui | cmd | cl, cheat | Hides the overlay. |
| cl_debugoverlay_toggle | cmd | cl, cheat | Toggles visibility of the debug overlay system. |
| cl_disable_ragdolls | false | cl, cheat |  |
| cl_display_game_events | false | cl, cheat |  |
| cl_draw_simulating_entities | false | cl, cheat |  |
| cl_drawcross | cmd | cl, cheat | Draws a cross at the given location  Arguments: x y z |
| cl_drawhud | true | cl, cheat | Enable the rendering of the hud |
| cl_drawline | cmd | cl, cheat | Draws line between two 3D Points.  Green if no collision  Red is collides with something  Arguments: x1 y1 z1 x2 y2 z2 |
| cl_dumpentity | cmd | cl, cheat | Dumps info about an entity |
| cl_ent_absbox | cmd | cl, cheat | Displays the total bounding box for the given entity(s) in green.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_actornames | cmd | cl, cheat | Displays the entity name for all entities that have ShouldDisplayInActorNames true in code |
| cl_ent_animgraph_debug | cmd | cl, cheat | Displays debug draws about the given entity(ies) animgraph  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_animgraph_record | cmd | cl, cheat | Toggles recording of animgraph replay of the given entity(s)  Arguments: entityName automaticallyOpenInAnimgraphEditor  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_attachments | cmd | cl, cheat | Displays the attachment points on an entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_bbox | cmd | cl, cheat | Displays the movement bounding box for the given entity(ies) in orange.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_call | cmd | cl, cheat | ent_call <funcname> <option:entname> calls function on current look target or filtername, checks on ent, then root, then mode, then map scope |
| cl_ent_clear_debug_overlays | cmd | cl, cheat | Clears all debug overlays |
| cl_ent_find | cmd | cl, cheat | Find and list all entities with classnames or targetnames that contain the specified substrings. Format: find_ent <substring> |
| cl_ent_find_index | cmd | cl, cheat | Display data for entity matching specified index. Format: find_ent_index <index> |
| cl_ent_grab | cmd | cl, cheat | grabs the object in front of the player. Options: -loose -multiple -toggle |
| cl_ent_hierarchy | cmd | cl, cheat | Prints the entity hierarchy tree rooted at the specified ent(s) |
| cl_ent_hitbox | cmd | cl, cheat | Displays the hitboxes for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_joints | cmd | cl, cheat | Displays the joint names + axes an entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_messages | cmd | cl, cheat | Toggles input/output message display for the selected entity(ies).  The name of the entity will be displayed as well as any messages that it sends or receives.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_name | cmd | cl, cheat | Displays the entity name |
| cl_ent_picker | cmd | cl, cheat | Toggles 'picker' mode.  When picker is on, the bounding box, pivot and debugging text is displayed for whatever entity the player is looking at.  Arguments: full - enables all debug information |
| cl_ent_pivot | cmd | cl, cheat | Displays the pivot for the given entity(ies).  (y=up=green, z=forward=blue, x=left=red).   Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_pivot_size | 20 | cl, a, cheat |  |
| cl_ent_remove | cmd | cl, cheat | Removes the given entity(s)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_remove_all | cmd | cl, cheat | Removes all entities of the specified type  Arguments:    {entity_name} / {class_name} |
| cl_ent_scale | cmd | cl, cheat | Scales entities. Arguments: <scale factor> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| cl_ent_scenehierarchy | cmd | cl, cheat | Prints the entity scenenode hierarchy tree rooted at the specified ent(s) |
| cl_ent_script_dump | cmd | cl, cheat | Dumps the names and values of this entity's script scope to the console  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_select | cmd | cl, cheat | Select or deselects the given entities(s) for later manipulation  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_setang | cmd | cl, cheat | Set entity angles |
| cl_ent_setname | cmd | cl, cheat | Sets the targetname of the given entity(s)  Arguments:    <new entity name> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| cl_ent_setpos | cmd | cl, cheat | Move entity to position |
| cl_ent_show_contexts | false | cl, cheat | Show entity contexts in ent_text display |
| cl_ent_show_damage | cmd | cl, cheat | Sets damage display mode.  When on, you will see the amount of damage dealt over the target's head. |
| cl_ent_showonlyattachment | 0 | cl, cheat |  |
| cl_ent_showonlyhitbox | -1 | cl, cheat |  |
| cl_ent_skeleton | cmd | cl, cheat | Displays the skeleton for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text | cmd | cl, cheat, vconsole_fuzzy | Displays text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text256 | cmd | cl, cheat | Displays text debugging information about the given entity(ies) [within 256 units of the player] on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text_clear | cmd | cl, cheat | Hide text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text_filter | cmd | cl, cheat | Set which ent_text filters you want |
| cl_ent_text_flags_active | -1 | cl, a, cheat |  |
| cl_ent_text_no_name_really_i_mean_it | false | cl, cheat |  |
| cl_ent_text_radius | cmd | cl, cheat | Displays text debugging information about the given entity(ies) [near the player] on top of the entity (See Overlay Text)  2 Arguments:    <Radius> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| cl_ent_text_sticky_add | cmd | cl, cheat | Adds to list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text_sticky_clear | cmd | cl, cheat | Clears the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text_sticky_dump | cmd | cl, cheat | Spews the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_text_sticky_remove | cmd | cl, cheat | Removes from the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_ungrab | cmd | cl, cheat | un-grabs all objects |
| cl_ent_vcollide_wireframe | cmd | cl, cheat | Displays the interpolated vcollide wireframe pm am entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_viewoffset | cmd | cl, cheat | Displays the eye position for the given entity(ies) in red.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_ent_visibility_traces | cmd | cl, cheat, vconsole_fuzzy | Displays visibility traces for the given entity  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_error_report_time | 0 | cl, release | Minimum time in seconds that must elapse before printing prediction error summary. 0 to disable. |
| cl_extrapolate | true | cl, cheat | Enable/disable extrapolation if interpolation history runs out. |
| cl_extrapolate_amount | 0.25 | cl, cheat | Set how many seconds the client will extrapolate entities for. |
| cl_eye_occlusion_debug | false | cl, cheat |  |
| cl_flushentitypacket | 0 | cheat | For debugging. Force the engine to flush an entity packet. |
| cl_frametime_summary_report_detailed | true | cl, release | When a perf report is dumped at the end of the session, should it be detailed? |
| cl_fullupdate | cmd | cheat | Force uncompressed update |
| cl_glow_brightness | 1 | cl, cheat | Brightness of player halos |
| cl_glow_item_far_b | 1 | cl, release |  |
| cl_glow_item_far_g | 0.4 | cl, release |  |
| cl_glow_item_far_r | 0.3 | cl, release |  |
| cl_graphics_driver_warning_dont_show_again | false | cl, archive release |  |
| cl_groups | cmd | cl, cheat | Show status of all spawn groups. |
| cl_hud_telemetry_frametime_poor | 100 | cl, archive release | Frame time greater than this is considered 'poor'. |
| cl_hud_telemetry_frametime_show | 1 | cl, archive release | Show frame time (FPS) in the HUD.  0=never, 1=only if poor, 2=always |
| cl_hud_telemetry_net_misdelivery_poor | 5 | cl, archive release | Packet delivery anomaly rate (0..100) higher than this is considered 'poor'. |
| cl_hud_telemetry_net_misdelivery_show | 1 | cl, archive release | Show packet delivery anomaly (loss or out-of-order) rate in the HUD.  0=never, 1=only in poor conditions, 2=always |
| cl_hud_telemetry_net_quality_graph_show | 0 | cl, archive release | Show packet jitter and netframe loss/reordering in the HUD.  0=never, 1=only in poor conditions, 2=always |
| cl_hud_telemetry_ping_poor | 100 | cl, archive release | Ping higher than this (ms) is considered 'poor'. |
| cl_hud_telemetry_ping_show | 0 | cl, archive release | Show ping in the HUD.  0=never, 1=only in poor conditions, 2=always |
| cl_hud_telemetry_serverrecvmargin_graph_show | 0 | cl, archive release | Show graph of the server recv margin in the HUD.  (How early/late user commands are arriving at the server before they are executed.)   0=never, 1=only when there are command queue problems, 2=always |
| cl_ignorepackets | false | cheat | Force client to ignore packets (for debugging). |
| cl_imgui_debug_entity | cmd | cl, cheat | Shows the entity browser, focused on the entity you specify.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cl_imgui_set_selection | cmd | cl, cheat | Sets ImGui selection |
| cl_imgui_set_status_text | cmd | cl, cheat | Sets ImGui header status text |
| cl_input_enable_raw_keyboard | false | release | Enable raw keyboard input |
| cl_interp | cmd | cl, release | Read the effective client simulation interpolation amount in terms of time. |
| cl_interp_hermite | true | cl, cheat | Set to zero do disable hermite interpolation. |
| cl_interp_ratio | 2 | cl, user | Sets the client simulation interpolation amount, in terms of server updates (final amount is cl_interp_ratio / cl_updaterate). |
| cl_interpolate_report | false | cl, archive | Enable to show interpolation profile timing |
| cl_jiggle_bone_debug | false | cheat | Display physics-based 'jiggle bone' debugging information |
| cl_jiggle_bone_debug_pitch_constraints | false | cheat | Display physics-based 'jiggle bone' debugging information |
| cl_jiggle_bone_debug_yaw_constraints | false | cheat | Display physics-based 'jiggle bone' debugging information |
| cl_jiggle_bone_invert | false | cheat |  |
| cl_jitter_bad_threshold_up | 20 | user | When upstream packet jitter in a frame exceeds this threshold (ms), the frame is considered to have 'irregular delivery'.  This is a derived value and should not be modified manually |
| cl_joystick_enabled | false | archive | Enable joystick input |
| cl_lagcompensation | true | cl, user | Perform server side lag compensation of weapon firing events. |
| cl_latch_report | false | cl, archive | Enable to output stats about latching |
| cl_leveloverview | 0 | cl, cheat |  |
| cl_lightquery_debug | false | cl, cheat |  |
| cl_lock_camera | false | cl, cheat |  |
| cl_max_particle_pvs_aabb_edge_length | 100 | release |  |
| cl_meep_mop_volume_trigger_max_count | 10 | cl, cheat | Number of triggers before meemop reaches full volume |
| cl_modifier_dump | cmd | cl, cheat | Display all modifiers for the unit: <entityindex/name> |
| cl_modifier_dump_list | cmd | cl, cheat | Dumps all modifiers that exist in the game |
| cl_modifier_dump_visible | cmd | cl, cheat | Print out non-hidden modifiers. |
| cl_modifier_spew_states | cmd | cl, cheat | Call to have the client spew their unit states affecting them, |
| cl_modifier_stringtable_dump | cmd | cl, cheat | Displays the contents of the modifier string table |
| cl_mouselook | true | cl, archive user, per_user, disconnected | Set to 1 to use mouse for look, 0 for keyboard look. Cannot be set while connected to a server. |
| cl_network_quality2 | -1 | cl, archive |  |
| cl_particle_retire_cost | 0 | cheat |  |
| cl_particle_simulate | true | cheat | Enables/Disables Particle Simulation |
| cl_pclass | 0 | cl, cheat | Dump entity by prediction classname. |
| cl_pdump | -1 | cl, cheat | Dump info about this entity to screen. |
| cl_phys_debug_callback_entities | false | cl, cheat | Print all entities that get touch callbacks. Each entity is printed only once. |
| cl_phys_enabled | true | cl, cheat | Enable all physics simulation |
| cl_phys_sleep_enable | true | cl, cheat | Enable sleeping for dynamic physics bodies. |
| cl_phys_stop_at_collision | 0 | cl, cheat |  |
| cl_pitchdown | 89 | cl, cheat |  |
| cl_pitchup | 89 | cl, cheat |  |
| cl_playerspraydisable | false | cl, archive | Disable player sprays. |
| cl_pred_always_latch | false | cl, release |  |
| cl_pred_print_every_cmd | false | cl, release | Print something every time we predict a command |
| cl_predict | true | cl, user, cheat | Perform client side prediction. |
| cl_prop_debug | cmd | cl, cheat | Toggle prop debug mode. If on, props will show colorcoded bounding boxes. Red means ignore all damage. White means respond physically to damage but never break. Green maps health in the range of 100 down to 1. |
| cl_querycache_stats | cmd | cl, cheat | Display status of the query cache (client only) |
| cl_ragdoll_limit | 20 | cl, archive | Maximum number of ragdolls to show (-1 disables limit) |
| cl_ragdoll_lru_debug | false | cl, rep, cheat |  |
| cl_removedecals | cmd | cl, cheat | Remove the decals from the entity under the crosshair. |
| cl_resend | 0.5 | release | Delay in seconds before the client will resend the 'connect' attempt |
| cl_rr_reloadresponsesystems | cmd | cl, cheat | Reload all response system scripts. |
| cl_save_animgraph_recording | cmd | cl, cheat | Saves all active animgraph recordings to disk  Arguments: automaticallyOpenInAnimgraphEditor |
| cl_scale_function_dump | cmd | cl, cheat | Print out all scale functions. |
| cl_script_add_debug_filter | cmd | cl, cheat | Add a filter to the game debug overlay |
| cl_script_add_watch | cmd | cl, cheat | Add a watch to the game debug overlay |
| cl_script_add_watch_pattern | cmd | cl, cheat | Add a watch to the game debug overlay |
| cl_script_attach_debugger | cmd | cl, cheat | Connect the vscript VM to the script debugger |
| cl_script_clear_watches | cmd | cl, cheat | Clear all watches from the game debug overlay |
| cl_script_debug | cmd | cl, cheat | Toggle the in-game script debug features |
| cl_script_dump_all | cmd | cl, cheat | Dump the state of the VM to the console |
| cl_script_find | cmd | cl, cheat | Find a key in the VM |
| cl_script_help | cmd | cl, cheat | Output help for script functions |
| cl_script_reload | cmd | cl, cheat | Reload scripts |
| cl_script_reload_code | cmd | cl, cheat | Execute a vscript file, replacing existing functions with the functions in the run script |
| cl_script_reload_entity_code | cmd | cl, cheat | Execute all of this entity's VScripts, replacing existing functions with the functions in the run scripts |
| cl_script_remove_debug_filter | cmd | cl, cheat | Remove a filter from the game debug overlay |
| cl_script_remove_watch | cmd | cl, cheat | Remove a watch from the game debug overlay |
| cl_script_remove_watch_pattern | cmd | cl, cheat | Remove a watch from the game debug overlay |
| cl_script_resurrect_unreachable | cmd | cl, cheat | Use the garbage collector to track down reference cycles |
| cl_script_trace_disable | cmd | cl, cheat | Turn off a particular trace output by file or function name |
| cl_script_trace_disable_all | cmd | cl, cheat | Turn off all trace output |
| cl_script_trace_disable_key | cmd | cl, cheat | Turn off a particular trace output by table/instance |
| cl_script_trace_enable | cmd | cl, cheat | Turn on a particular trace output by file or function name |
| cl_script_trace_enable_all | cmd | cl, cheat | Turn on all trace output |
| cl_script_trace_enable_key | cmd | cl, cheat | Turn on a particular trace output by table/instance |
| cl_showents | cmd | cl, cheat | Dump entity list to console. |
| cl_showerror | 0 | cl, release | Show prediction errors, 2 for above plus detailed field deltas, 3 to filter out serverside known prediction errors, -entindex for specific entity. |
| cl_showfps | 0 | cl, release | Draw fps meter at top of screen (1 = fps, 2 = smooth fps, 3 = server MS, 4 = Show FPS and Log to file ) |
| cl_showmem | 0 | cl, release | Draw approximate memory use at top of screen |
| cl_showpos | 0 | cl, cheat, release | Draw current position, angle, and velocity on side of screen |
| cl_skel_constraints_enable | true | rep, cheat |  |
| cl_skeleton_instance_smear_boneflags | false | cl, cheat | Smear boneflags across the model.  Costs computation, but tests to make sure your bone flags are consistent. |
| cl_snd_new_visualize | false | cl, cheat | Displays soundevent name played at it's 3d position |
| cl_soundscape_flush | cmd | cl, cheat, server_can_execute | Flushes the client side soundscapes |
| cl_spewserializers | cmd | cheat | Spew serializers |
| cl_test_list_entities | cmd | cl, cheat | test-list entities |
| cl_tickpacket_desired_queuelength | 1 | user | This value, multiplied by the tick interval, is added to cl_tickpacket_recvmargin_desired to obtain the effective desired recv margin. |
| cl_tickpacket_recvmargin_spew_interval | 0 | release |  |
| cl_ticks_warning_level | 0 | release | Print a message about problems with ticks and interpolation.  0=never, 1=warnings, 2=all, even if hidden by interpolation |
| cl_ticktiming | cmd | norecord, release | <interval>} [summary|detail]  Print timing stats now, or set report interval |
| cl_timeout | 30 | archive | After this many seconds without receiving a packet from the server, the client will disconnect itself |
| cl_updaterate | 20 | cl, archive user | Number of packets per second of updates you are requesting from the server |
| cl_usercmd_max_per_movemsg | 4 | release | max number of CUserCmds to send in one client move message |
| cl_voice_transmit_lobby | false | cl, archive release |  |
| clear | cmd | norecord, release | Clear console output. |
| clearall | cmd | norecord, release | Clear console output from all views. |
| cli_ent_attachments | cmd | cl, cheat | Displays the interpolated attachment points on an entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cli_ent_hitbox | cmd | cl, cheat | Displays the skeleton for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cli_ent_pivot | cmd | cl, cheat | Displays the interpolated pivot for the given entity(ies).  (y=up=green, z=forward=blue, x=left=red).   Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cli_ent_skeleton | cmd | cl, cheat | Displays the skeleton for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| cli_ent_vcollide_wireframe | cmd | cl, cheat | Displays the interpolated vcollide wireframe pm am entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| clientport | 0 | release | If non-zero, client binds port to specific address.  Usually you should leave this blank to use a different random system-assigned port for each connection. |
| closecaption | false | cl, archive user | Enable close captioning. |
| collect_entity_model_name | cmd | sv, cheat | Collect model names of the entities you're pointing at |
| commentary | false | sv, a | Desired commentary mode state. |
| commentary_finishnode | cmd | sv |  |
| con_enable | false | archive per_user | Allows the console to be activated. |
| condump | cmd | release | dump the text currently in the console to condumpXX.log |
| connect | cmd | release | Connect to a remote server. |
| connect_hltv | cmd | release | Connect to a remote HLTV server. |
| consoletool | cmd | norecord, release | Open a VConsole subtool. |
| cq_buffer_bloat_msecs_max | 120 | replicated release | Server will not allow the client to buffer up more than N ms of commands. |
| cq_logging | false | sv, release | command queue logging of events. |
| cq_logging_interval | 0 | sv, release | command queue logging per player stats every N seconds, 0 to disable. |
| cq_max_starved_substitute_commands | 4 | sv, release | Server will stop generating substitute commands if client hasn't sent one, after N in a row |
| cq_print_every_command | false | sv, release | print every command as we execute it |
| crash | cmd | cheat | Crash the client. Optional parameter -- type of crash:0: read from NULL  1: write to NULL  2: force an Assert  3: infinite loop  4: stack buffer overrun  5: multiple asserts across multiple threads |
| crash_error | cmd | cheat | Cause the engine to crash by Plat_FatalError on main thread (Debug!!) |
| crash_error_job | cmd | cheat | Cause the engine to crash by Plat_FatalError on job thread (Debug!!) |
| crash_error_thread | cmd | cheat | Cause the engine to crash by Plat_FatalError on non-main thread (Debug!!) |
| crash_job | cmd | cheat | Cause the engine to crash in a job thread (Debug!!) |
| crash_thread | cmd | cheat | Cause the engine to crash in a brand new non-main thread (Debug!!) |
| create_flashlight | cmd | sv, cheat |  |
| create_radius_damage | cmd | sv, cheat | Causes radius damage where you're looking, at the passed in radius. |
| csm_bias_override_0 | 1 | cheat |  |
| csm_bias_override_1 | 1 | cheat |  |
| csm_bias_override_2 | 1 | cheat |  |
| csm_bias_override_3 | 1 | cheat |  |
| csm_cascade0_override_dist | -1 | cheat |  |
| csm_cascade1_override_dist | -1 | cheat |  |
| csm_cascade2_override_dist | -1 | cheat |  |
| csm_cascade3_override_dist | -1 | cheat |  |
| csm_cascade_viewdir_shadow_bias_scale | 2 | cheat |  |
| csm_max_dist_between_caster_and_receiver | 15000 | cheat | default pushback |
| csm_max_visible_dist | 7500 | cheat |  |
| csm_res_override_0 | 0 | cheat |  |
| csm_res_override_1 | 0 | cheat |  |
| csm_res_override_2 | 0 | cheat |  |
| csm_res_override_3 | 0 | cheat |  |
| csm_shadow_worldview_align_x_to_u | true | cheat |  |
| csm_shadow_worldview_shear_align_z_to_v | true | cheat |  |
| csm_split_log_scalar | 0.85 | cheat |  |
| csm_sst_max_visible_dist | 2000 | cheat |  |
| csm_sst_pushback_distance | 1500 | cheat | default pushback |
| csm_sst_shadow_focus_region_maxz | 2000 | cheat |  |
| csm_sst_shadow_focus_region_minz | -2000 | cheat |  |
| csm_viewdir_shadow_bias | 0 | cheat |  |
| csm_viewmodel_farz | 30 | cheat |  |
| csm_viewmodel_max_shadow_dist | 21 | cheat |  |
| csm_viewmodel_max_visible_dist | 1000 | cheat |  |
| csm_viewmodel_nearz | 0.5 | cheat |  |
| cvarlist | cmd | release | Show the list of convars/concommands. |
| cyclevar | cmd | norecord, release | Cycle through specified convar values. |
| db_default_bot_difficulty | 1 | cl, archive | Used to cache the last set bot difficulty across runs |
| deadlock_early_development_warning_disabled | false | cl, archive | Disable the early dev build message |
| deadlock_get_old_builds | cmd | cl, release | Usage: deadlock_get_old_builds [author_account_id] - if omitted, will use your account. |
| deadlock_post_match_survey_disabled | false | cl, archive | Disable the early post match survey |
| debug_takedamage_summaries | false | sv, cheat |  |
| debug_visibility_monitor | 0 | sv, cheat |  |
| debugoverlay_cycle_domain | cmd | sv, cheat | Toggles visibility of the debug overlay system. |
| debugoverlay_cycle_state | cmd | sv, cheat | Toggles visibility of the debug overlay system. |
| debugoverlay_dashboard | cmd | sv, cheat | Makes the debug overlay dashboard visible. |
| debugoverlay_force_respect_ttl | false | cheat | Force respect TTL even when clearing scopes |
| debugoverlay_hide_imgui | cmd | sv, cheat | Hides the overlay. |
| debugoverlay_show_text_outline | false | cheat | Toggle display of box around text |
| debugoverlay_text_scale | 1 | a, cheat | Scale of the text used for 3d display |
| debugoverlay_toggle | cmd | sv, cheat | Toggles visibility of the debug overlay system. |
| default_fov | 70 | cl, cheat |  |
| demo_flush | false | archive | Flush writing the demo file every network update |
| demo_goto | cmd | release | Skips to location in demo. |
| demo_gotomark | cmd | release | Skips the current demo playback to the marked tick |
| demo_gototick | cmd | release | Skips to a tick in demo. |
| demo_info | cmd | release | Print information about currently playing demo. |
| demo_marktick | cmd | release | Marks the current demo playback tick for later use |
| demo_pause | cmd | release | Pauses demo playback. |
| demo_quitafterplayback | false | release | Quits game after demo playback. |
| demo_recordcommands | true | cheat | Record commands typed at console into .dem files. |
| demo_resume | cmd | release | Resumes demo playback. |
| demo_timescale | cmd | release | Sets demo replay speed. |
| demo_togglepause | cmd | release | Toggles demo playback. |
| demolist | cmd | release | Print demo sequence list. |
| developer | 0 | release | Set developer message level. |
| differences | cmd | release | Show all convars which are not at their default values (optional restricted to specific flags). |
| disable_dynamic_prop_loading | false | sv, cheat | If non-zero when a map loads, dynamic props won't be loaded |
| disconnect | cmd | release | Disconnect from server |
| display_game_events | false | sv, cheat |  |
| dlight_debug | cmd | cl, cheat | Creates a dlight in front of the player |
| dota_enable_spatial_audio | false | release | Flag to enable spatial audio in Dota 2. |
| dota_spatial_audio_mix | 1 | release | Mix value to blend spatial and non-spatial audio in Dota 2. |
| drawcross | cmd | sv, cheat | Draws a cross at the given location  Arguments: x y z |
| drawline | cmd | sv, cheat | Draws line between two 3D Points.  Green if no collision  Red is collides with something  Arguments: x1 y1 z1 x2 y2 z2 |
| dsp_dist_max | 1440 | cheat, demo |  |
| dsp_dist_min | 0 | cheat, demo |  |
| dsp_off | false | cheat |  |
| dsp_volume | 0.8 | archive demo |  |
| dump_entity_report | cmd | cl, cheat | List all client-side entities in the scene |
| dump_hero_names | cmd | cl, cheat | Lists all heroes by their technical names |
| dump_panorama_css_properties | cmd | release | Prints out all valid panorama CSS properties and their documentation |
| dump_panorama_events | cmd | release | print panorama event types and their documentation |
| dumpparticlelist | cmd | release | Print out information on existing particle systems |
| echo | cmd | server_can_execute | Echo text to console. |
| echoln | cmd | release | Echo the command arguments on the console |
| enable_boneflex | true | cl, archive |  |
| engine_low_latency_sleep_after_client_tick | false | release | When r_low_latency is enabled, this moves the low latency sleep on tick frames to happen after client simulation. |
| engine_no_focus_sleep | 20 | archive |  |
| engine_show_frame_pacing | false | release |  |
| english | true | cl, user | If set to 1, running the english language set of assets. |
| ent_absbox | cmd | sv, cheat | Displays the total bounding box for the given entity(s) in green.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_actornames | cmd | sv, cheat | Displays the entity name for all entities that have ShouldDisplayInActorNames true in code |
| ent_actornames_font | Consolas | sv, cl, rep, cheat | ent_actornames font name |
| ent_actornames_fontsize | 24 | sv, cl, rep, cheat | ent_actornames font size |
| ent_animgraph_debug | cmd | sv, cheat | Displays debug draws about the given entity(ies) animgraph  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_animgraph_record | cmd | sv, cheat | Toggles recording of animgraph replay of the given entity(s)  Arguments: entityName automaticallyOpenInAnimgraphEditor  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_animgraph_setvar | cmd | sv, cheat | Sets a variable on the animgraph of the given entity(s)  Arguments:   <varname>=<value> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| ent_attachments | cmd | sv, cheat | Displays the attachment points on an entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_autoaim | cmd | sv, cheat | Displays the entity's autoaim radius.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_bbox | cmd | sv, cheat | Displays the movement bounding box for the given entity(ies) in orange.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_bonemergeplayer | cmd | sv, cheat | Bonemerge the player onto the entity under the crosshairs |
| ent_call | cmd | sv, cheat | ent_call <funcname> <option:entname> calls function on current look target or filtername, checks on ent, then root, then mode, then map scope |
| ent_clear_debug_overlays | cmd | sv, cheat | Clears all debug overlays |
| ent_create | cmd | sv, cheat, vconsole_fuzzy | Creates an entity of the given designer or subclass name where the player is looking. |
| ent_find | cmd | sv, cheat | Find and list all entities with classnames or targetnames that contain the specified substrings. Format: find_ent <substring> |
| ent_find_index | cmd | sv, cheat | Display data for entity matching specified index. Format: find_ent_index <index> |
| ent_fire | cmd | sv, cheat, vconsole_fuzzy | Usage:    ent_fire <target> [action] [value] [delay] |
| ent_fire_output | cmd | sv, cheat, vconsole_fuzzy | Usage:    ent_fire_output <target> [output name] [value] [delay] |
| ent_grab | cmd | sv, cheat | grabs the object in front of the player. Options: -loose -multiple -toggle |
| ent_hierarchy | cmd | sv, cheat | Prints the entity hierarchy tree rooted at the specified ent(s) |
| ent_hitbox | cmd | sv, cheat | Displays the hitboxes for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_info | cmd | sv, cheat | Usage:    ent_info <class name> |
| ent_joints | cmd | sv, cheat | Displays the joint names + axes an entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_kill | cmd | sv, cheat | Kills the given entity(s)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_messages | cmd | sv, cheat | Toggles input/output message display for the selected entity(ies).  The name of the entity will be displayed as well as any messages that it sends or receives.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_messages_draw | false | sv, cl, rep, cheat | Visualizes all entity input/output activity. |
| ent_name | cmd | sv, cheat | Displays the entity name |
| ent_orient | cmd | sv, cheat | Orient the specified entity to match the player's angles. By default, only orients target entity's YAW. Use the 'allangles' option to orient on all axis.  Format: ent_orient <entity name> <optional: allangles> |
| ent_picker | cmd | sv, cheat | Toggles 'picker' mode.  When picker is on, the bounding box, pivot and debugging text is displayed for whatever entity the player is looking at.  Arguments: full - enables all debug information |
| ent_pivot | cmd | sv, cheat | Displays the pivot for the given entity(ies).  (y=up=green, z=forward=blue, x=left=red).   Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_pivot_size | 20 | sv, a, cheat |  |
| ent_rbox | cmd | cl, cheat | Displays the total bounding box for the given entity(s) in green.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_remove | cmd | sv, cheat | Removes the given entity(s)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_remove_all | cmd | sv, cheat | Removes all entities of the specified type  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_rotate | cmd | sv, cheat | Rotates an entity by a specified # of degrees |
| ent_scale | cmd | sv, cheat | Scales entities. Arguments: <scale factor> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| ent_scenehierarchy | cmd | sv, cheat | Prints the entity scenenode hierarchy tree rooted at the specified ent(s) |
| ent_script_dump | cmd | sv, cheat | Dumps the names and values of this entity's script scope to the console  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_select | cmd | sv, cheat | Select or deselects the given entities(s) for later manipulation  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_setang | cmd | sv, cheat | Set entity angles |
| ent_setname | cmd | sv, cheat | Sets the targetname of the given entity(s)  Arguments:    <new entity name> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| ent_setpos | cmd | sv, cheat | Move entity to position |
| ent_show_contexts | false | sv, cheat | Show entity contexts in ent_text display |
| ent_show_damage | cmd | sv, cheat | Sets damage display mode.  When on, you will see the amount of damage dealt over the target's head. |
| ent_show_response_criteria | cmd | sv, cheat | Print, to the console, an entity's current criteria set used to select responses.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_showonlyattachment | 0 | sv, cheat |  |
| ent_skeleton | cmd | sv, cheat | Displays the skeleton for the given entity(ies).  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_skeleton_duration | 0 | sv, cl, rep, cheat | Duration of ent_skeleton display |
| ent_teleport | cmd | sv, cheat | Teleport the specified entity to where the player is looking.  Format: ent_teleport <entity name> |
| ent_text | cmd | sv, cheat, vconsole_fuzzy | Displays text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text256 | cmd | sv, cheat | Displays text debugging information about the given entity(ies) [within 256 units of the player] on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text_clear | cmd | sv, cheat | Hide text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text_filter | cmd | sv, cheat | Set which ent_text filters you want |
| ent_text_flags_active | -1 | sv, a, cheat |  |
| ent_text_no_name_really_i_mean_it | false | sv, cheat |  |
| ent_text_radius | cmd | sv, cheat | Displays text debugging information about the given entity(ies) [near the player] on top of the entity (See Overlay Text)  2 Arguments:    <Radius> <{entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at}> |
| ent_text_sticky_add | cmd | sv, cheat | Adds to list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text_sticky_clear | cmd | sv, cheat | Clears the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text_sticky_dump | cmd | sv, cheat | Spews the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_text_sticky_remove | cmd | sv, cheat | Removes from the list of names to display text debugging information about the given entity(ies) on top of the entity (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_ungrab | cmd | sv, cheat | un-grabs all objects |
| ent_vcollide_wireframe | cmd | sv, cheat | Displays the interpolated vcollide wireframe pm am entity.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_viewoffset | cmd | sv, cheat | Displays the eye position for the given entity(ies) in red.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| ent_visibility_traces | cmd | sv, cheat, vconsole_fuzzy | Displays visibility traces for the given entity  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| entity_log_load_unserialize | 0 | sv, cl, rep, cheat | Output unserialization of entities on map load. 0 - off, 1 - client/server, 2 - server, 3 - client |
| escape | cmd | release, clientcmd_can_execute | Escape key pressed. |
| exec | cmd | norecord, release | Execute a cfg file |
| exec_async | cmd | cheat, norecord | Execute a cfg file over time |
| execifexists | cmd | norecord, release | Execute a cfg file if file exists |
| execute_command_every_frame | 0 | cheat |  |
| experimental_citadel_botmatch_tick_rate_override | 0 | sv, cl, rep, release |  |
| experimental_citadel_tick_rate_override | 0 | sv, cl, rep, release |  |
| explode | cmd | sv, cheat | Kills the player with explosive damage |
| explodevector | cmd | sv, cheat | Kills a player applying an explosive force. Usage: explodevector <player> <x value> <y value> <z value> |
| fadein | cmd | sv, cheat | fadein {time r g b}: Fades the screen in from black or from the specified color over the given number of seconds. |
| fadeout | cmd | sv, cheat | fadeout {time r g b}: Fades the screen to black or to the specified color over the given number of seconds. |
| find | cmd | release | Find concommands with the specified string in their name/help text. |
| findflags | cmd | release | Find concommands by flags. |
| firetarget | cmd | sv, cheat |  |
| firstperson | cmd | cl, release, execute_per_tick | Switch to firstperson camera. |
| fish_debug | false | cl, cheat | Show debug info for fish |
| fish_dormant | false | sv, rep, cheat | Turns off interactive fish behavior. Fish become immobile and unresponsive. |
| fog_color | -1.000000 -1.000000 -1.000000 | cl, cheat |  |
| fog_colorskybox | -1.000000 -1.000000 -1.000000 | cl, cheat |  |
| fog_enable | true | cl, cheat | Enable fog |
| fog_enableskybox | true | cl, cheat |  |
| fog_end | -1 | cl, cheat |  |
| fog_endskybox | -1 | cl, cheat |  |
| fog_hdrcolorscale | -1 | cl, cheat |  |
| fog_hdrcolorscaleskybox | -1 | cl, cheat |  |
| fog_maxdensity | -1 | cl, cheat |  |
| fog_maxdensityskybox | -1 | cl, cheat |  |
| fog_override | 0 | cl, cheat | Overrides the map's fog settings (-1 populates fog_ vars with map's values) |
| fog_override_color | cmd | cheat | Sets the fog color override |
| fog_override_enable | false | cheat | Use fog_override convars instead of world fog data |
| fog_override_end | 3500 | cheat |  |
| fog_override_exponent | 2 | cheat |  |
| fog_override_max_density | 0.4 | cheat |  |
| fog_override_start | 1000 | cheat |  |
| fog_start | -1 | cl, cheat |  |
| fog_startskybox | -1 | cl, cheat |  |
| fov_desired | 75 | cl, archive user | Sets the base field-of-view. |
| fps_max | 400 | archive release | Frame rate limiter.  0=no limit.  Does not apply to dedicated server. |
| fps_max_tools | 120 | archive | Additional frame rate limit while in tools mode and a window other than the game window has focus. Note that fps_max still applies, this only allows the maximum frame rate for tools mode to be lower. 0=no tools specific limit. |
| fps_max_ui | 120 | archive | Frame rate limiter while the game UI is displayed.  0=no limit.  Does not apply to dedicated server. |
| fs_fake_read_delay_ms | 0 | release | Add N ms of delay to every low-level read operation, to simulate a slow disk |
| fs_report_sync_opens | 0 | release | 0:Off, 1:Always, 2:Not during load |
| fs_spew_readfieldlist | cmd | cheat | index <threshold bytes>: spew changes to ent index, optionally only spewing if update is > than threshold bytes |
| func_break_max_pieces | 15 | sv, a, rep |  |
| g_debug_angularsensor | false | sv, cheat |  |
| g_debug_constraint_sounds | false | sv, cheat | Enable debug printing about constraint sounds. |
| g_debug_ragdoll_visualize | false | cl, cheat |  |
| gameinstructor_dump_open_lessons | cmd | cl, cheat | Gives a list of all currently open lessons. |
| gameinstructor_dump_run_lesson_counts | cmd | cl, cheat | Gives a list of lessons that been completed or shown |
| gameinstructor_enable | true | cl, archive release | Display in game lessons that teach new players. |
| gameinstructor_find_errors | false | cl, cheat | Set to 1 and the game instructor will run EVERY scripted command to uncover errors. |
| gameinstructor_verbose | 0 | cl, cheat | Set to 1 for standard debugging or 2 (in combo with gameinstructor_verbose_lesson) to show update actions. |
| gameinstructor_verbose_lesson | 0 | cl, cheat | Display more verbose information for lessons have this name. |
| gameui_hide | cmd | release | Hides the game UI |
| getpos | cmd | cl, cheat | dump position and angles to the console |
| getpos_exact | cmd | cl, cheat | dump origin and angles to the console |
| gameui_hide |  |  | Hides the game UI |
| give_oriented | cmd | sv, vconsole_fuzzy | Give item oriented to player angles.  Arguments: <item_name> |
| givecurrentammo | cmd | sv, cheat | Give a supply of ammo for current weapon. |
| giveitem | cmd | sv, vconsole_fuzzy | Give item to player.  Arguments: <item_name> |
| gl_clear_gray | false | cl, cheat | Clear the back buffer to gray every frame. |
| gl_clear_randomcolor | false | cl, cheat | Clear the back buffer to random colors every frame. Helps spot open seams in geometry. |
| global_set | cmd | sv, cheat | global_set <globalname> <state>: Sets the state of the given env_global (0 = OFF, 1 = ON, 2 = DEAD). |
| glow_use_tolerance | 0.85 | cl, rep, cheat |  |
| god | cmd | sv, cheat | Toggle by default, or 0 to disable and 1 to enable. Player becomes invulnerable. |
| grep | cmd | release | grep line for pattern, print out matching lines only |
| groups | cmd | sv, cheat | Show status of all spawn groups. |
| help | cmd | release | Find help about a convar/concommand. |
| +herochatwheel | cmd | cl, release | Opens hero chatwheel menu while held |
| hide_party_code | false | cl, archive | When set, this will hide the party code in the client |
| hideconsole | cmd | norecord, release | Hide the console. |
| host_framerate | 0 | release | Set to lock per-frame time elapse. |
| host_readconfig_ignore_userconfig | false | cheat | Whether we should ignore the user config file for reading/writing. |
| host_timescale | 1 | rep, cheat | Prescale the clock by this amount. |
| host_timescale_dec | cmd | cheat | Decrement the timescale by one step |
| host_timescale_inc | cmd | cheat | Increment the timescale by one step |
| host_writeconfig | cmd | release | Saves out the user config values. |
| hostfile | host.txt | sv, release | The HOST file to load. |
| hostip | 0 | release | Host game server ip |
| hostname | unnamed | release | Hostname for server. |
| hostname_in_client_status | false | release | Show server hostname in client status. |
| hostport | 27015 | release | Host game server port |
| hud_damagemeter | false | cl, cheat |  |
| hud_fastswitch | 0 | cl, archive |  |
| hud_free_cursor | -1 | cl, release | If -1 use the hud default, otherwise 0 is disabled, 1 is enabled |
| hud_free_cursor_toggle | cmd | cl, release | Toggles free cursor convar. |
| hud_minimap_spectator_fow_team_view_amber | cmd | cl, release | While a spectator, view team amber's minimap view |
| hud_minimap_spectator_fow_team_view_both_teams | cmd | cl, release | While a spectator, view both teams' minimap view |
| hud_minimap_spectator_fow_team_view_sapphire | cmd | cl, release | While a spectator, view team sapphire's minimap view |
| ' hud_minimap_spectator_fow_team_view_target_team | cmd | cl, release | While a spectator and viewing a player, view team their minimap view |
| hurtme | cmd | sv, cheat | Hurts the player.  Arguments: <health to lose> |
| ik_debug_chain_to_filter_by | 0 | sv, cl, rep, cheat |  |
| ik_enable | true | cheat | Enable IK. |
| ik_hinge_debug_bone_index | -1 | sv, cl, rep, cheat |  |
| imgui_debug_entity | cmd | sv, cheat | Shows the entity browser, focused on the entity you specify.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| imgui_default_font_size | 20 | a, cheat | Default imgui font size |
| imgui_set_selection | cmd | sv, cheat | Sets ImGui selection |
| imgui_set_status_text | cmd | sv, cheat | Sets ImGui header status text |
| impulse | cmd | cl, release | Triggers impulse command |
| +in_ability_ping | cmd | cl, release | Ping button pressed |
| incrementvar | cmd | norecord, release | Increment specified convar value. |
| input_button_code_is_scan_code_scd | true | archive per_user | Bind keys based on keyboard position instead of key name |
| input_filter_relative_analog_inputs | false | cl, archive |  |
| input_forceuser | -1 | cheat | Force user input to this split screen player. |
| interesting_events_draw_debug | false | sv, cheat | When enabled, draws a sphere representing active events |
| ip | 0 | release | Overrides IP for multihomed hosts |
| iv_debugbone | 0 | release | Debug bone name for interpolation spew of CAnimationState. |
| joy_advanced | false | cl, archive |  |
| joy_advaxisr | 0 | cl, archive |  |
| joy_advaxisu | 0 | cl, archive |  |
| joy_advaxisv | 0 | cl, archive |  |
| joy_advaxisx | 0 | cl, archive |  |
| joy_advaxisy | 0 | cl, archive |  |
| joy_advaxisz | 0 | cl, archive |  |
| joy_axisbutton_threshold | 0.3 | archive | Analog axis range before a button press is registered. |
| joy_axisr_deadzone | 0.15 | archive per_user |  |
| joy_axisr_relative | false | archive per_user |  |
| joy_axisu_deadzone | 0.15 | archive per_user |  |
| joy_axisu_relative | false | archive per_user |  |
| joy_axisv_deadzone | 0.15 | archive per_user |  |
| joy_axisv_relative | false | archive per_user |  |
| joy_axisx_deadzone | 0.15 | archive per_user |  |
| joy_axisx_relative | false | archive per_user |  |
| joy_axisy_deadzone | 0.15 | archive per_user |  |
| joy_axisy_relative | false | archive per_user |  |
| joy_axisz_deadzone | 0.15 | archive per_user |  |
| joy_axisz_relative | false | archive per_user |  |
| joy_circle_correct_mode | 1 | cl, archive per_user |  |
| joy_circle_correct_mode_vehicle | 2 | cl, archive per_user |  |
| joy_display_input | false | cl, archive |  |
| joy_forward_sensitivity | 1 | cl, archive per_user |  |
| joy_movement_stick | false | cl, archive per_user | Which stick controls movement (0 is left stick) |
| joy_name | joystick | cl, archive |  |
| joy_pitch_sensitivity | 3 | cl, archive per_user |  |
| joy_pitchsensitivity | 1 | cl, archive per_user |  |
| joy_response_look | 0 | cl, archive per_user |  |
| joy_response_move | 9 | cl, archive per_user |  |
| joy_side_sensitivity | 1 | cl, archive per_user |  |
| joy_sidesensitivity | 1 | cl, archive |  |
| joy_yaw_sensitivity | 3 | cl, archive per_user |  |
| joy_yawsensitivity | -1 | cl, archive per_user |  |
| joystick | false | cl, archive | True if the joystick is enabled, false otherwise. |
| key_findbinding | cmd | release | Find key bound to specified command string. |
| key_listboundkeys | cmd | release | List bound keys with bindings. |
| kick | cmd | norecord, release | Kick a player by name. |
| kickid | cmd | norecord, release | Kick a player by userid or uniqueid, with a message. |
| kickid_hltv | cmd | norecord, release | Kick a player by userid or uniqueid, with a message. |
| kill | cmd | sv, cheat | Kills the player with generic damage |
| killvector | cmd | sv, cheat | Kills a player applying force. Usage: killvector <player> <x value> <y value> <z value> |
| labelled_debug_helper_arc_segments | 20 | sv, cl, rep, cheat |  |
| labelled_debug_helper_enabled | true | sv, cl, rep, cheat |  |
| labelled_debug_helper_scale | 1 | sv, cl, rep, cheat |  |
| labelled_debug_helper_show_position | false | sv, cl, rep, cheat |  |
| labelled_debug_helper_show_text | true | sv, cl, rep, cheat |  |
| labelled_debug_helper_skeleton_show_bone_names | true | sv, cl, rep, cheat |  |
| last_viewed_announce_id | -1 | cl, archive | Tracks the last announcement ID viewed so we can know when new announcements are available |
| lb_barnlight_shadowmap_scale | 1 | release | Scale for computed barnlight shadowmap size |
| lb_shadow_map_cull_empty_mixed | false | cheat | Don't render shadows for mixed shadowmaps with no dynamics objects in view |
| lb_shadow_map_culling | true | cheat |  |
| lightquery_debug_direct_lighting | true | sv, cl, rep, cheat |  |
| lightquery_debug_indirect_lighting | true | sv, cl, rep, cheat |  |
| listdemo | cmd | release | List demo file contents. |
| log | cmd | release | off >. |
| log_color | cmd | norecord, release | Set the color of a logging channel. |
| log_dumpchannels | cmd | norecord, release | Dumps information about all logging channels. |
| log_flags | cmd | norecord, release | Set the flags on a logging channel. |
| log_level | cmd | norecord, release | Set the spew level of a logging channel. |
| log_verbosity | cmd | norecord, release | Set the verbosity of a logging channel. |
| logic_npc_counter_debug | false | sv, rep, cheat |  |
| m_pitch | 0.022 | cl, archive user, per_user | Mouse pitch factor. |
| m_yaw | 0.022 | cl, archive user, per_user | Mouse yaw factor. |
| map | cmd | release, vconsole_fuzzy, vconsole_set_focus | map <mapname> :Load a new map. |
| map_enable_portrait_worlds | cmd | cl, cheat | Enables/disables portrait worlds |
| maps | cmd | release | Displays list of maps. |
| markup_group_ent_bbox | cmd | sv, cheat | markup_group_ent_bbox <markup_group name> -> toggle ent_bbox for all members of the named markup group |
| markup_group_ent_text | cmd | sv, cheat | markup_group_ent_text <markup_group name> -> toggle ent_text for all members of the named markup group |
| markup_group_spew | cmd | sv, cheat | Spew all current markup groups and their members |
| mat_colcorrection_forceentitiesclientside | false | cl, cheat | Forces color correction entities to be updated on the client |
| mat_fullbright | 0 | cheat | Debug rendering modes |
| mat_lpv_luxels | false | cheat |  |
| mat_luxels | false | cheat |  |
| mat_max_lighting_complexity | 8 | cheat |  |
| mat_overdraw | 0 | cheat | Visualize overdraw |
| mat_overdraw_color | 0.075000 0.150000 0.300000 | cheat |  |
| mat_shading_complexity | false | cheat | Visualize shading complexity |
| mat_shading_complexity_color | 1.000000 0.500000 0.250000 | cheat |  |
| mat_shading_complexity_max_instruction_count | 1024 | cheat |  |
| mat_shading_complexity_max_register_count | 128 | cheat |  |
| mat_shadowmap_luxels | false | cheat |  |
| mat_show_distance_field | 0 | cheat | 0=Off, 1=Visualize trace from camera, 2=Visualize occlusion, 3=Visualize far field trace from camera |
| mat_tonemap_bloom_scale | -1 | cheat |  |
| mat_tonemap_bloom_start_value | -1 | cheat |  |
| mat_tonemap_force_accelerate_exposure_down | -1 | cheat |  |
| mat_tonemap_force_average_lum_min | -1 | cheat | Override. Old default was 3.0 |
| mat_tonemap_force_log_lum_max | -1 | cheat |  |
| mat_tonemap_force_log_lum_min | -1 | cheat |  |
| mat_tonemap_force_max | -1 | cheat |  |
| mat_tonemap_force_min | -1 | cheat |  |
| mat_tonemap_force_percent_bright_pixels | -1 | cheat | Override. Old value was 1.0 |
| mat_tonemap_force_percent_target | -1 | cheat | Override. Old default was 45. |
| mat_tonemap_force_rate | -1 | cheat |  |
| mat_tonemap_force_scale | 0 | cheat |  |
| mat_tonemap_force_use_alpha | -1 | cheat |  |
| mat_tonemap_uncap_exposure | 0 | cheat |  |
| mat_wireframe | 0 | cheat | 0=Off, 1=Surface Wireframe, 2=Transparent Wireframe |
| mesh_calculate_curvature_smooth_invert | false | sv, cl, rep, cheat |  |
| mesh_calculate_curvature_smooth_pass_count | 3 | sv, cl, rep, cheat |  |
| mesh_calculate_curvature_smooth_weight | 1 | sv, cl, rep, cheat |  |
| mobile_fps_increase_during_charging | false | archive | MOBILE_FPS_CONTROL: If true we increase framerate limit while charging |
| mobile_fps_increase_during_touch | true | archive | MOBILE_FPS_CONTROL: If true we increase framerate limit during touch |
| mobile_fps_limit | 30 | archive | MOBILE_FPS_CONTROL: Mobile FPS limit - 15, 30, 60 |
| mod_status | cmd | cl, release | <Account ID> |
| model_default_preview_sequence_name | 0 | sv, cl, a, rep |  |
| modifier_aura_debug | false | sv, cl, rep, cheat | Set to 1 to draw the radii of all active auras |
| modifier_create | cmd | sv, cheat, vconsole_fuzzy | Creates a test modifier on unit: modifier_create <entityindex> <modifiername> <duration> |
| modifier_dump | cmd | sv, cheat | Display all modifiers for the unit: <entityindex/name> |
| modifier_dump_list | cmd | sv, cheat | Dumps all modifiers that exist in the game |
| modifier_dump_visible | cmd | sv, cheat | Print out non-hidden modifiers. |
| modifier_remove | cmd | sv, cheat, vconsole_fuzzy | Removes the first modifier that matches the name from a unit: modifier_remove <entityindex> <modifiername> |
| modifier_spew_states | cmd | sv, cheat | Call to have the client spew their unit states affecting them, |
| modifier_stringtable_dump | cmd | sv, cheat | Displays the contents of the modifier string table |
| modifier_test_scripted_event | cmd | sv, cheat | Tests firing a scripted event |
| modifier_test_scripted_event_end | cmd | sv, cheat | Tests firing ending a scripted event |
| motdfile | motd.txt | sv, release | The MOTD file to load. |
| mouse_inverty | false | cl, archive user |  |
| mp_disable_autokick | cmd | sv, release | Prevents a userid from being auto-kicked |
| mp_forcecamera | 0 | sv, cl, rep, release | Restricts spectator modes for dead players |
| mp_friendlyfire | false | sv, cl, nf, rep, release | Allows team members to injure other members of their team |
| mp_restartgame | 0 | sv, release | If non-zero, game will restart in the specified number of seconds |
| multvar | cmd | norecord, release | Multiply specified convar value. |
| name | unnamed | archive per_user |  |
| nav_add_to_selected_set | cmd | sv, cheat | Add current area to the selected set. |
| nav_add_to_selected_set_by_id | cmd | sv, cheat | Add specified area id to the selected set. |
| nav_avoid | cmd | sv, cheat | Toggles the 'avoid this area when possible' flag used by the AI system. |
| nav_avoid_obstacles | true | sv, cheat |  |
| nav_begin_deselecting | cmd | sv, cheat | Start continuously removing from the selected set. |
| nav_begin_drag_deselecting | cmd | sv, cheat | Start dragging a selection area. |
| nav_begin_drag_selecting | cmd | sv, cheat | Start dragging a selection area. |
| nav_begin_selecting | cmd | sv, cheat | Start continuously adding to the selected set. |
| nav_bfs_debug | 0 | sv, cheat |  |
| nav_clear_attribute | cmd | sv, cheat | Remove given nav attribute from all areas in the selected set. |
| nav_clear_attributes | cmd | sv, cheat | Clear all nav attributes of selected area. |
| nav_clear_selected_set | cmd | sv, cheat | Clear the selected set. |
| nav_corner_adjust_adjacent | 18 | cheat | radius used to raise/lower corners in nearby areas when raising/lowering corners. |
| nav_create_indirect_connection | cmd | sv, cheat | Create a connection between the selected area and the area pointed at by the crosshair. |
| nav_create_indirect_connection_from_to | cmd | sv, cheat | Create a connection between the current 'from' and 'to' locations. |
| nav_create_indirect_connection_set_from | 0.000000 0.000000 0.000000 | sv, cheat | Set the 'from' location of an indirect connection. |
| nav_create_indirect_connection_set_from_using_editpos | cmd | sv, cheat | Set the 'from' location of an indirect connection to be the current edit pos of nav_edit. |
| nav_create_indirect_connection_set_to | 0.000000 0.000000 0.000000 | sv, cheat | Set the 'to' location of an indirect connection. |
| nav_create_indirect_connection_set_to_using_editpos | cmd | sv, cheat | Set the 'to' location of an indirect connection to be the current edit pos of nav_edit. |
| nav_curve_alt | false | sv, cheat |  |
| nav_curve_iter | 0 | sv, cheat |  |
| nav_curve_lock | -1 | sv, cheat |  |
| nav_curve_max_step | 10 | sv, cheat |  |
| nav_curve_set | -1 | sv, cheat |  |
| nav_curve_step | 0.02 | sv, cheat |  |
| nav_debug_blocked | false | sv, cheat |  |
| nav_delete | cmd | sv, cheat | Deletes the currently highlighted Area. |
| nav_delete_all_hull | cmd | sv, cheat | Deletes all areas with given hull category. |
| nav_delete_marked | cmd | sv, cheat | Deletes the currently marked Area (if any). |
| nav_disconnect | cmd | sv, cheat | To disconnect two Areas, mark an Area, highlight a second Area, then invoke the disconnect command. This will remove all connections between the two Areas. |
| nav_draw_area_connections | false | sv, cheat |  |
| nav_draw_area_filled | true | sv, cheat |  |
| nav_draw_area_gravity | false | sv, cheat |  |
| nav_draw_area_ground | false | sv, cheat |  |
| nav_draw_area_hull_support | false | sv, cheat |  |
| nav_draw_area_ids | false | sv, cheat |  |
| nav_draw_area_inset_margin | 0 | sv, cheat |  |
| nav_draw_area_normal | false | sv, cheat |  |
| nav_draw_area_should_be_destroyed | false | sv, cheat |  |
| nav_draw_area_split_by_nav_link_mgr | false | sv, cheat |  |
| nav_draw_area_split_by_obstacle_mgr | false | sv, cheat |  |
| nav_draw_area_ztest | false | sv, cheat |  |
| nav_draw_attribute_dynamic | 0 | sv, cheat | Draw all nav areas with this dynamic attribute |
| nav_draw_attribute_game | 0 | sv, cheat | Draw all nav areas with this game attribute |
| nav_draw_blocked | true | sv, cheat |  |
| nav_draw_blocked_connections | false | sv, cheat |  |
| nav_draw_connected_area_radius | 1000 | sv, cheat |  |
| nav_draw_externally_created | false | sv, cheat |  |
| nav_draw_indirect_connections | false | sv, cheat |  |
| nav_draw_jump_links | false | sv, cheat |  |
| nav_draw_limit | 300 | sv, cheat | The maximum number of areas to draw in edit mode |
| nav_draw_link_alignment | false | sv, cheat |  |
| nav_draw_links | false | sv, cheat |  |
| nav_draw_markup | true | sv, cheat |  |
| nav_draw_mesh | true | sv, cheat |  |
| nav_draw_mesh_grid | false | sv, cheat | Draw the mesh's spatial grid structure around the edit cursor position. |
| nav_draw_mesh_offset | 1 | sv, cheat | Vertical offset for drawing the mesh (useful for flat planes where the mesh is often a fixed offset from the physical ground |
| nav_draw_space_boundary | false | sv, cheat |  |
| nav_draw_space_cells | false | sv, cheat |  |
| nav_draw_space_fly | false | sv, cheat |  |
| nav_draw_space_neighbors | false | sv, cheat |  |
| nav_draw_space_portals | false | sv, cheat |  |
| nav_draw_space_radius | 0 | sv, cheat |  |
| nav_draw_space_swim | false | sv, cheat |  |
| nav_edit | 0 | sv, cheat | Set to one to interactively edit the Navigation Mesh. Set to zero to leave edit mode. |
| nav_edit_validate | false | sv, cheat | Validate navmesh structures. |
| nav_end_deselecting | cmd | sv, cheat | Stop continuously removing from the selected set. |
| nav_end_drag_deselecting | cmd | sv, cheat | Stop dragging a selection area. |
| nav_end_drag_selecting | cmd | sv, cheat | Stop dragging a selection area. |
| nav_end_selecting | cmd | sv, cheat | Stop continuously adding to the selected set. |
| nav_find_occluded_node_nozup_use_raycast | true | sv, cheat |  |
| nav_gen_add_jumps | true | cheat |  |
| nav_gen_agent_radius_buffer | 0.5 | cheat | Buffer to add to agent radius before passing to nav gen |
| nav_gen_clip_polys_to_clearance | true | cheat |  |
| nav_gen_clip_polys_to_clearance_debug | false | cheat |  |
| nav_gen_connect_allow_multiple | true | cheat |  |
| nav_gen_connect_angle | 0.75 | cheat |  |
| nav_gen_connect_angle_ignore_z | true | cheat |  |
| nav_gen_connect_dist_a | 1 | cheat |  |
| nav_gen_connect_dist_b | 1.5 | cheat |  |
| nav_gen_connect_dist_z_mult | 0.5 | cheat |  |
| nav_gen_connect_overlap | 0.5 | cheat |  |
| nav_gen_degen_limit | 0.001 | cheat |  |
| nav_gen_false | false | cheat | Always false |
| nav_gen_island_removal | false | cheat |  |
| nav_gen_island_removal_all_hulls | true | cheat |  |
| nav_gen_join_nonzup | true | cheat |  |
| nav_gen_jump_connection_min_overlap_ratio | 1 | cheat | Minimum edge overlap required for jump connection consideration as a percentage of agent radius |
| nav_gen_markup_split_expand | 2 | cheat |  |
| nav_gen_markup_split_tol_base | 1 | cheat |  |
| nav_gen_markup_split_tol_nonav | 1 | cheat |  |
| nav_gen_markup_split_tol_nonentity | 8 | cheat |  |
| nav_gen_match_ground | false | cheat |  |
| nav_gen_max_bottleneck_width | 128 | cheat |  |
| nav_gen_max_bottleneck_width_do_clip | true | cheat |  |
| nav_gen_max_edge_len | 512 | cheat |  |
| nav_gen_max_edge_len_do_clip | true | cheat |  |
| nav_gen_max_edge_len_split_tol | 24 | cheat |  |
| nav_gen_opt_to_quads | true | cheat |  |
| nav_gen_opt_to_quads_angle_limit | 8 | cheat |  |
| nav_gen_opt_to_quads_num_steps | 6 | cheat |  |
| nav_gen_opt_to_quads_planar_deviation_limit | 4 | cheat |  |
| nav_gen_opt_to_quads_se_limit_end | 0.1 | cheat |  |
| nav_gen_opt_to_quads_se_limit_start | 0.00001 | cheat |  |
| nav_gen_opt_to_quads_weld_limit_end | 0.01 | cheat |  |
| nav_gen_opt_to_quads_weld_limit_start | 0 | cheat |  |
| nav_gen_oriented_angle_tol | 15 | cheat | Max abrupt orientation difference an NPC can tolerate when moving through the mesh (degrees). |
| nav_gen_oriented_max_region_range | 30 | cheat | Max orientation range allowed within a region before it gets further split. |
| nav_gen_remove_vertical_polys | true | cheat |  |
| nav_gen_split_boundary_polys | false | cheat |  |
| nav_gen_split_multi_connection_polys | true | cheat |  |
| nav_gen_split_multi_connection_polys_tol | 0.01 | cheat |  |
| nav_gen_true | true | cheat | Always true |
| nav_gen_vertical_limit | 88 | cheat |  |
| nav_genrt_debug | false | sv, cheat |  |
| nav_genrt_no_splice | false | sv, cheat |  |
| nav_genrt_no_split | false | sv, cheat |  |
| nav_genrt_step | -1 | sv, cheat |  |
| nav_lower_drag_volume_max | cmd | sv, cheat | Lower the top of the drag select volume. |
| nav_lower_drag_volume_min | cmd | sv, cheat | Lower the bottom of the drag select volume. |
| nav_mark | cmd | sv, cheat | Marks the Area or Ladder under the cursor for manipulation by subsequent editing commands. |
| nav_mark_attribute | cmd | sv, cheat | Set nav attribute for all areas in the selected set. |
| nav_max_vis_delta_list_length | 64 | cheat |  |
| nav_obstacle_genrt | false | sv, cheat |  |
| nav_obstacle_validate | false | sv, cheat |  |
| nav_obstruction_draw | 0 | sv, cheat |  |
| nav_obstruction_draw_change | false | sv, cheat |  |
| nav_obstruction_draw_dist | -1 | sv, cheat |  |
| nav_obstruction_draw_island | 0 | sv, cheat |  |
| nav_obstruction_draw_island_hull | -1 | sv, cheat |  |
| nav_obstruction_draw_movefail_blocking | false | sv, cheat |  |
| nav_path_debug | false | sv, cheat |  |
| nav_path_debug_compute_with_open_goal | 0 | sv, cheat |  |
| nav_path_draw_areas | false | sv, cheat |  |
| nav_path_draw_arrow | true | sv, cheat |  |
| nav_path_draw_climb_segments | true | sv, cheat |  |
| nav_path_draw_connected_areas | false | sv, cheat |  |
| nav_path_draw_ground_segments | true | sv, cheat |  |
| nav_path_draw_jump_segments | true | sv, cheat |  |
| nav_path_draw_ladder_segments | true | sv, cheat |  |
| nav_path_draw_link_segments | true | sv, cheat |  |
| nav_path_draw_tick | 0 | sv, cheat |  |
| nav_path_fixup_climb_up_segments | true | sv, cheat |  |
| nav_path_fixup_gap_segments | false | sv, cheat |  |
| nav_path_jump_process_debug | false | sv, cheat |  |
| nav_path_optimize | true | sv, cheat |  |
| nav_path_optimize_portals | true | sv, cheat |  |
| nav_path_optimizer_debug | 0 | sv, cheat |  |
| nav_path_record_draw_last_fail | false | sv, cheat |  |
| nav_path_record_enable | 1 | sv, cheat |  |
| nav_pathfind_debug_log | 0 | sv, cheat |  |
| nav_pathfind_draw | 0 | sv, cheat |  |
| nav_pathfind_draw_blocked | 0 | sv, cheat |  |
| nav_pathfind_draw_costs | false | sv, cheat |  |
| nav_pathfind_draw_fail | 0 | sv, cheat |  |
| nav_pathfind_draw_total_costs | false | sv, cheat |  |
| nav_pathfind_inadmissable_heuristic_factor | 1 | sv, cheat |  |
| nav_pathfind_multithread | false | sv, cheat |  |
| nav_raise_drag_volume_max | cmd | sv, cheat | Raise the top of the drag select volume. |
| nav_raise_drag_volume_min | cmd | sv, cheat | Raise the bottom of the drag select volume. |
| nav_recall_selected_set | cmd | sv, cheat | Re-selects the stored selected set. |
| nav_remove_from_selected_set | cmd | sv, cheat | Remove current area from the selected set. |
| nav_select_allow_blocked | true | sv, cheat | When selecting an area under nav_edit, allow area marked as blocked. |
| nav_select_area_id | -1 | sv, cheat | Select nav area with matching ID. |
| nav_select_block_id | -1 | sv, cheat | Select nav space block with matching ID. |
| nav_select_hull | 0 | sv, cheat | Restrict area selection to areas that can support a hull of the given category |
| nav_select_radius | cmd | sv, cheat | Adds all areas in a radius to the selection set |
| nav_select_with_attribute | cmd | sv, cheat | Selects areas with the given attribute. |
| nav_show_area_connections | true | sv, cheat | Show connections to selected area when true |
| nav_show_area_info_font | Consolas | sv, cheat |  |
| nav_show_area_info_font_size | -1 | sv, cheat |  |
| nav_show_area_info_font_voffset | -11 | sv, cheat |  |
| nav_show_area_verts | true | sv, cheat | Show area vertex positions |
| nav_show_area_water_info | true | sv, cheat |  |
| nav_show_potentially_visible | 0 | cheat | Show areas that are potentially visible from the current nav area |
| nav_smooth_constrain_results | true | sv, cheat |  |
| nav_smooth_constrain_results_relax | 0.006 | sv, cheat |  |
| nav_smooth_constrain_spring | 2 | sv, cheat |  |
| nav_smooth_constrain_spring_relax | 0.01 | sv, cheat |  |
| nav_smooth_draw_accel | 0 | sv, cheat |  |
| nav_smooth_draw_boundary | 0 | sv, cheat |  |
| nav_smooth_draw_calc | false | sv, cheat |  |
| nav_smooth_draw_constraint_spline | false | sv, cheat |  |
| nav_smooth_draw_constraint_spring | 0 | sv, cheat |  |
| nav_smooth_draw_speed | 0 | sv, cheat |  |
| nav_smooth_enable | true | sv, cheat |  |
| nav_smooth_relax | true | sv, cheat |  |
| nav_smooth_relax_use_timesteps | false | sv, cheat |  |
| nav_smooth_spring_const_override | -1 | sv, cheat |  |
| nav_smooth_spring_enable | true | sv, cheat |  |
| nav_smooth_spring_factor_deriv | 0 | sv, cheat |  |
| nav_smooth_spring_factor_dist | 0 | sv, cheat |  |
| nav_smooth_spring_factor_speed | 0 | sv, cheat |  |
| nav_smooth_spring_forward_dist_base | 50 | sv, cheat |  |
| nav_smooth_spring_forward_dist_time_limit | 1 | sv, cheat |  |
| nav_smooth_spring_max_dist | 36 | sv, cheat |  |
| nav_smooth_spring_tension_max_override | -1 | sv, cheat |  |
| nav_smooth_spring_timestep_factor_accel | 100 | sv, cheat |  |
| nav_smooth_spring_timestep_factor_speed | 100 | sv, cheat |  |
| nav_smooth_spring_timestep_max | 0.5 | sv, cheat |  |
| nav_smooth_spring_timestep_min | 0.1 | sv, cheat |  |
| nav_smooth_spring_yaw_rotation_speed | 50 | sv, cheat |  |
| nav_smooth_spring_yaw_threshold | 20 | sv, cheat |  |
| nav_smooth_use_opt | true | sv, cheat |  |
| nav_space_select_dist | 1000 | sv, cheat |  |
| nav_split | cmd | sv, cheat | To split an Area into two, align the split line using your cursor and invoke the split command. |
| nav_split_show_line | false | sv, cheat | Show the free split line. |
| nav_store_selected_set | cmd | sv, cheat | Stores the current selected set for later retrieval. |
| nav_test_area_gravity | false | sv, cheat |  |
| nav_test_bfs_lattice_dist_0 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_dist_1 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_dist_2 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_hex | false | sv, cheat | Demonstrates searching hexagonal lattice over nav mesh. |
| nav_test_bfs_lattice_mark | 2 | sv, cheat |  |
| nav_test_bfs_lattice_simple | false | sv, cheat |  |
| nav_test_bfs_lattice_spacing_0 | 24 | sv, cheat |  |
| nav_test_bfs_lattice_spacing_1 | 48 | sv, cheat |  |
| nav_test_bfs_lattice_spacing_2 | 96 | sv, cheat |  |
| nav_test_bfs_simple | false | sv, cheat |  |
| nav_test_boundary_zone_circle | 0 | sv, cheat |  |
| nav_test_boundary_zone_force | false | sv, cheat |  |
| nav_test_boundary_zone_grid_dim | 90 | sv, cheat |  |
| nav_test_boundary_zone_path | 0 | sv, cheat |  |
| nav_test_boundary_zone_rays | 100 | sv, cheat |  |
| nav_test_boundary_zone_rays_margin | -1 | sv, cheat |  |
| nav_test_boundary_zone_rays_random | false | sv, cheat |  |
| nav_test_boundary_zone_sphere | 0 | sv, cheat |  |
| nav_test_curve_opt | 0 | sv, cheat |  |
| nav_test_detour | false | sv, cheat |  |
| nav_test_find_nearest | false | sv, cheat | Calculate the nearest point on the navmesh to the trace point.  Uses selection from nav_select_hull. |
| nav_test_find_nearest_clear | false | sv, cheat | Calculate the nearest point on the navmesh to the trace point.  Uses selection from nav_select_hull. |
| nav_test_find_random_connected | false | sv, cheat | Demonstrates finding random points that are connected in the nav mesh to the start point. |
| nav_test_find_random_connected_dist_max | 1000 | sv, cheat |  |
| nav_test_find_random_connected_dist_min | 100 | sv, cheat |  |
| nav_test_find_z | 0 | sv, cheat |  |
| nav_test_force_npc_repath | false | sv, cheat |  |
| nav_test_genrt | false | sv, cheat |  |
| nav_test_genrt_place | false | sv, cheat |  |
| nav_test_getareaoverlapping_gravity | false | sv, cheat |  |
| nav_test_getnearestnav_gravity | false | sv, cheat |  |
| nav_test_level_hull | cmd | sv, cheat | Find entities that intrude into the nav mesh.  List those entities in console output, and display bounding boxes around them for a while. |
| nav_test_level_hull_move | cmd | sv, cheat |  |
| nav_test_multi_connection | false | sv, cheat |  |
| nav_test_npc_area | 0 | sv, cheat |  |
| nav_test_npc_collision | 0 | sv, cheat |  |
| nav_test_npc_collision_range | 250 | sv, cheat |  |
| nav_test_npc_collision_show_geometry | false | sv, cheat |  |
| nav_test_path | false | sv, cheat | Calculate and draw a path from player/camera position to the test position. |
| nav_test_path_expansion_search | 0 | sv, cheat | Extend nav_test_path by doing an expansion search on that path.  Convar value defines dist. |
| nav_test_path_lock_goal | false | sv, cheat | Lock the pathfinding goal to the current intersection point. |
| nav_test_path_lock_start | false | sv, cheat | Lock the pathfinding start to the current intersection point. |
| nav_test_path_move | false | sv, cheat |  |
| nav_test_path_opt | true | sv, cheat | Enable path optimization for nav_edit_path paths. |
| nav_test_path_opt_transitions | false | sv, cheat |  |
| nav_test_path_return | false | sv, cheat | Calculate a return path from cursor position to the path calculated by nav_test_path. |
| nav_test_path_space | 0 | sv, cheat | Should nav_test_path test 3d navigation?  1 = space to space, 2 = multi-modal space/ground |
| nav_test_path_space_fly | true | sv, cheat | Test flight paths |
| nav_test_path_space_swim | true | sv, cheat | Test swim paths |
| nav_test_ray_space | 0 | sv, cheat |  |
| nav_test_rays | false | sv, cheat |  |
| nav_test_smooth | false | sv, cheat |  |
| nav_test_smooth_extern_push | 0 | sv, cheat |  |
| nav_test_smooth_in_speed | 120 | sv, cheat |  |
| nav_test_smooth_in_yaw | 0 | sv, cheat |  |
| nav_test_smooth_path_speed | -1 | sv, cheat |  |
| nav_test_smooth_separating_dist | -1 | sv, cheat |  |
| nav_test_smooth_spring_const | -1 | sv, cheat |  |
| nav_test_smooth_spring_tension_max | -1 | sv, cheat |  |
| nav_test_spline | 0 | sv, cheat |  |
| nav_test_split_obstacle | 0 | sv, cheat |  |
| nav_test_split_obstacle_dirty | false | sv, cheat |  |
| nav_test_split_obstacle_leave | false | sv, cheat |  |
| nav_test_split_obstacle_size | 30 | sv, cheat |  |
| nav_test_split_obstacle_update_pos | true | sv, cheat |  |
| nav_toggle_deselecting | cmd | sv, cheat | Start or stop continuously removing from the selected set. |
| nav_toggle_in_selected_set | cmd | sv, cheat | Remove current area from the selected set. |
| nav_toggle_selected_set | cmd | sv, cheat | Toggles all areas into/out of the selected set. |
| nav_toggle_selecting | cmd | sv, cheat | Start or stop continuously adding to the selected set. |
| nav_unmark | cmd | sv, cheat | Clears the marked Area or Ladder. |
| nav_validate | 0 | cheat | Level of validation for nav system.  Higher will be slower. |
| nav_volume_debug | 0 | sv, cheat | Draw or print debug information about nav volume queries. |
| navlocal_constrain | true | sv, cheat |  |
| navlocal_debug | 0 | sv, cheat |  |
| navlocal_debug_constraint | 0 | sv, cheat |  |
| navlocal_debug_isect | 0 | sv, cheat |  |
| navlocal_debug_island_calc | 0 | sv, cheat |  |
| navlocal_debug_obstructions | 0 | sv, cheat |  |
| navlocal_lead_in_dist | 64 | sv, cheat |  |
| navlocal_lead_out_dist | 18 | sv, cheat |  |
| navlocal_path_tight_buffer | 2 | sv, cheat |  |
| navlocal_start_solid_calc_path | false | sv, cheat |  |
| navspace_create_water_smooth_connections | true | sv, cheat |  |
| navspace_create_water_transition_connections | true | sv, cheat |  |
| navspace_debug_pathfind | -1 | sv, cheat |  |
| navspace_debug_stringpull | 1 | sv, cheat |  |
| navspace_debug_trace | 0 | sv, cheat |  |
| navspace_debug_transition_calc | 0 | sv, cheat |  |
| navspace_draw_water_changes | 0 | sv, cheat | Draw changes in water volumes |
| navspace_path_use_water_level_locator | true | sv, cheat |  |
| nav_gen_opt_to_quads_weld_limit_start | 0 | cheat |  |
| net_channels | cmd | release | Shows net channel info |
| net_connections_stats | cmd | release | Print detailed network statistics for each network connection |
| net_fakeclear | cmd | release | Clear all simulated network conditions |
| net_fakejitter | cmd | release | Shortcut to set jitter net options.  Run with no arguments for usage. |
| net_fakelag | cmd | release | Shortcut to set both FakePacketLag_Recv and FakePacketLag_Send net options |
| net_fakeloss | cmd | release | Shortcut to set both FakePacketLoss_Recv and FakePacketLoss_Send net options |
| net_fakestatus | cmd | release | Print current simulated network condifions |
| net_limit_sv_recv_max_message_size_kb | 32 | release | Server will reject message larger than N kb |
| net_limit_sv_recv_segments_per_packet | 50 | release | Server will reject packets with more than N segments |
| net_limit_sv_recvbuffer_kb | 128 | release | Server will not buffer more than N kb from connected clients |
| net_limit_sv_recvbuffer_msg | 100 | release | Server will not buffer more than N messages from connected clients |
| net_listallmessages | cmd | cheat | List all registered net messages |
| net_messageinfo | cmd | cheat | Display info about a message (by classname or id) |
| net_option | cmd | release | Get or set SteamNetworkingSockets options such as fake packet lag and loss |
| net_print_sdr_ping_times | cmd | release | Print current ping times to SDR points of presence, and selected route |
| net_public_adr | 0 | release | For servers behind NAT/DHCP meant to be exposed to the public internet, this is the public facing ip address string: ('x.x.x.x' ) |
| net_showudp | false | release | Dump UDP packets summary to console |
| net_showudp_remoteonly | true | release | Dump non-loopback udp only |
| net_status | cmd | release | Shows current network status |
| net_validatemessages | cmd | cheat | Activates/deactivates net message validation |
| nextdemo | cmd | release | Play next demo in sequence. |
| noclip | cmd | sv, cheat | Toggle. Player becomes non-solid and flies.  Optional argument of 0 or 1 to force enable/disable |
| noclip_fixup | true | sv, cheat |  |
| notarget | cmd | sv, cheat | Toggle. Player becomes hidden to NPCs. |
| npc_ability_range_debug | cmd | sv, cheat, vconsole_fuzzy | Draws range indicators for abilities for the given NPC(s).  Uses the NPCs enemy for range drawing.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_bodylocations | cmd | sv, cheat, vconsole_fuzzy | Displays labelled body locations of NPCs.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_combat | cmd | sv, cheat | Displays text debugging information about the squad and enemy of the selected NPC  (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_conditions | cmd | sv, cheat, vconsole_fuzzy | Displays all the current AI conditions that an NPC has in the overlay text.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_conditions_text | cmd | sv, cheat, vconsole_fuzzy | Outputs text debugging information to the console about the all condition gathering for the selected NPC current schedule  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_create | cmd | sv, cheat, vconsole_fuzzy | Creates an NPC of the given type where the player is looking (if the given NPC can actually stand at that location).    Arguments: [npc_class_name] [name of npc (optional) ] [addon type (optional) ] [name of addon (optional) ] |
| npc_create_aimed | cmd | sv, cheat, vconsole_fuzzy | Creates an NPC aimed away from the player of the given type where the player is looking (if the given NPC can actually stand at that location).  Note that this only works for npc classes that are already in the world.  You can not create an entity that doesn't have an instance in the level.  Arguments: {npc_class_name} |
| npc_create_or_teleport_warn_on_nonav | true | sv, cheat | Warn if the created or teleported npc is off nav. |
| npc_damage | cmd | sv, cheat | Deals the target damage by the given amount |
| npc_destroy | cmd | sv, cheat, vconsole_fuzzy | Removes the given NPC(s) from the universe  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_destroy_unselected | cmd | sv, cheat | Removes all NPCs from the universe that aren't currently selected |
| npc_enemies | cmd | sv, cheat, vconsole_fuzzy | Shows memory of NPC.  Draws an X on top of each memory.  Eluded entities drawn in blue (don't know where it went)  Unreachable entities drawn in green (can't get to it)  Current enemy drawn in red  Current target entity drawn in magenta  All other entities drawn in pink  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_go | cmd | sv, cheat | Selected NPC(s) will go to the location that the player is looking (shown with a purple box)  Arguments: <start x y z> <goal x y z> |
| npc_go_last | cmd | sv, cheat | Go to the last position you told an NPC to go. |
| npc_go_loop | cmd | sv, cheat | Toggles whether the selected NPC(s) will loop between the last set of waypoints you used 'npc go' on. |
| npc_go_loop_clear_waypoints | cmd | sv, cheat | Clear waypoints for npc_go_loop. |
| npc_go_no_arrow | false | sv, a | Don't draw the go arrow of selected NPCs |
| npc_go_random | cmd | sv, cheat | Sends all selected NPC(s) to a random node.  Arguments:    -none- |
| npc_go_update_path | cmd | sv, cheat | Selected NPC(s) will go to the location that the player is looking (shown with a purple box), WITHOUT CHANGING SCHEDULE!  Arguments: [dest_fly] |
| npc_kill | cmd | sv, cheat, vconsole_fuzzy | Kills the given NPC(s)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_kill_unselected | cmd | sv, cheat | Properly kills all NPCs from the universe that aren't currently selected |
| npc_relationships | cmd | sv, cheat, vconsole_fuzzy | Displays the relationships between this NPC and all others.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_reportstate | cmd | sv, cheat | Outputs the current state of the NPC |
| npc_reset | cmd | sv, cheat | Reloads schedules for all NPC's from their script files  Arguments: -none- |
| npc_route | cmd | sv, cheat, vconsole_fuzzy | Displays the current route of the given NPC as a line on the screen.  Waypoints along the route are drawn as small cyan rectangles.  Line is color coded in the following manner:  Blue - path to a node  Cyan - detour around an object (triangulation)  Red - jump  Maroon - path to final target position  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_scripted_commands | cmd | sv, cheat, vconsole_fuzzy | Displays the state of scripted commands on the NPC  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_select | cmd | sv, cheat, vconsole_fuzzy | Select or deselects the given NPC(s) for later manipulation.  Selected NPC's are shown surrounded by a red translucent box  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_squads | cmd | sv, cheat | Obsolete.  Replaced by npc_combat |
| npc_steering | cmd | sv, cheat, vconsole_fuzzy | Displays the steering obstructions of the NPC (used to perform local avoidance)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_steering_all | cmd | sv, cheat | Displays the steering obstructions of all NPCs (used to perform local avoidance) |
| npc_stop_moving | cmd | sv, cheat | Selected NPC(s) will stop moving.  Arguments: [asap] |
| npc_task_text | cmd | sv, cheat, vconsole_fuzzy | Outputs text debugging information to the console about the all the tasks + break conditions of the selected NPC current schedule  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_tasks | cmd | sv, cheat, vconsole_fuzzy | Displays detailed text debugging information about the all the tasks of the selected NPC current schedule (See Overlay Text)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| npc_teleport | cmd | sv, cheat | Selected NPC will teleport to the location that the player is looking (shown with a purple box)  Arguments: -none- |
| npc_viewcone | cmd | sv, cheat, vconsole_fuzzy | Displays the viewcone of the NPC (where they are currently looking and what the extents of there vision is)  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| option_duck_method | false | cl, archive user, per_user | Input toggle control |
| orb_timing_debug | false | sv, release | Spew a bunch of timing info about when orbs are hit and claimed into the log. |
| panorama_debugger_theme | Light | cl, archive |  |
| panorama_focus_world_panels | false | cl, archive | when set request key focus when a world panel is enabled |
| panorama_joystick_enabled | false | archive | Enable panorama joystick input |
| particle_test_attach_attachment | 0 | sv, cheat | Attachment index for attachment mode |
| particle_test_attach_mode | follow_attachment | sv, cheat | Possible Values: 'start_at_attachment', 'follow_attachment', 'start_at_origin', 'follow_origin' |
| particle_test_create | cmd | sv, cheat | Creates the named particle system where the player is looking.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| particle_test_destroy | cmd | sv, cheat | Destroys all particle systems matching the specified name.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| particle_test_file | 0 | sv, cheat | Name of the particle system to dynamically spawn |
| particle_test_start | cmd | sv, cheat | Dispatches the test particle system with the parameters specified in particle_test_file,  particle_test_attach_mode and particle_test_attach_param on the entity the player is looking at.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| particle_test_stop | cmd | sv, cheat | Stops all particle systems on the selected entities.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| particles_multiplier | 1 | cheat | Multiply # of rendered particles by this for perf testing |
| party_refresh | cmd | cl, release | Refreshes the party panel |
| password | 0 | archive norecord, server_cant_query | Current server access password |
| pause | cmd | release | Toggle the server pause state. |
| pestilence_drone_healthbar_pos | 80 | cl, cheat |  |
| phys_debug_showdefaultmaterial | false | cheat | If enabled, surfaces with default material are highlighted in physics debug geometry. |
| phys_dynamic_scaling | true | sv, cl, rep, cheat |  |
| phys_expensive_shape_threshold | 6 | cl, cheat |  |
| phys_highlight_expensive_objects | false | cheat | Highlight expensive physics objects |
| phys_highlight_expensive_objects_strength | 0.02 | cheat | Highlight expensive physics objects strength |
| phys_joint_teleport | true | sv, cheat | Teleport joint anchors if connected to world |
| phys_length_damping_ratio | 2 | sv, cheat | Spring damping ratio for length constraint |
| phys_length_frequency | 5 | sv, cheat | Spring stiffness for length constraint |
| phys_mark_debug | cmd | sv, cheat | Mark object for debug |
| phys_shoot | cmd | sv, cheat | Shoots a phys object. |
| phys_use_block_solver | true | sv, cheat | Use block solving for constraint entities |
| phys_visualize_traces | false | sv, cl, rep, cheat |  |
| ping_quick_response | cmd | cl, release | Responds to the last ping message received |
| ping_wheel_phrase_0 | 1 | cl, archive per_user |  |
| ping_wheel_phrase_1 | 2 | cl, archive per_user |  |
| ping_wheel_phrase_2 | 4 | cl, archive per_user |  |
| ping_wheel_phrase_3 | 34 | cl, archive per_user |  |
| ping_wheel_phrase_4 | 18 | cl, archive per_user |  |
| ping_wheel_phrase_5 | 5 | cl, archive per_user |  |
| ping_wheel_phrase_6 | 42 | cl, archive per_user |  |
| ping_wheel_phrase_7 | 6 | cl, archive per_user |  |
| pixelvis_debug | cmd | cheat | Dump debug info |
| play | cmd | server_can_execute | Play a sound. |
| playcast | cmd | release | Play a broadcast |
| playdemo | cmd | release | Play a recorded demo file (.dem ). |
| player0_using_joystick | false | archive |  |
| player_ammobalancing_debug | false | sv, cheat |  |
| player_debug_off_nav | false | sv, cheat |  |
| player_debug_print_damage | false | sv, cheat | When true, print amount and type of all damage received by player to console. |
| playsoundscape | cmd | cl, cheat | Forces a soundscape to play |
| print_changed_convars | cmd | release | Prints all convars that have changed from their default value |
| private_lobby_create | cmd | cl, release | Creates a private lobby party |
| prop_debug | cmd | sv, cheat | Toggle prop debug mode. If on, props will show colorcoded bounding boxes. Red means ignore all damage. White means respond physically to damage but never break. Green maps health in the range of 100 down to 1. |
| prop_debug_collision | false | sv, cheat | Highlights props based on their collision group: COLLISION_GROUP_PROPS(white), COLLISION_GROUP_INTERACTIVE_DEBRIS(green), COLLISION_GROUP_DEBRIS and will return to COLLISION_GROUP_INTERACTIVE_DEBRIS on sleeping(bright red), COLLISION_GROUP_DEBRIS permanently (dark red), COLLISION_GROUP_DEBRIS(blue), OTHER(grey) |
| prop_dynamic_create | cmd | sv, cheat | Creates a dynamic prop with a specific .vmdl aimed away from where the player is looking.  Arguments: {.vmdl name} |
| prop_physics_create | cmd | sv, cheat | Creates a physics prop with a specific .vmdl aimed away from where the player is looking.  Arguments: {.vmdl name} |
| pulse_list_graphs | cmd | cheat | List all the active pulse graph instances |
| pulse_open_graph_id | cmd | cheat | Open a specific graph instance by id |
| pulse_print_graph_execution_history | cmd | cheat | Prints the execution history of a graph by filename or instanceid |
| pvs_debugentity | -1 | sv, release | Verbose spew for this entity when doing IsInPVS computation. |
| pvs_flowtype | 0 | sv, release | Flow through spawn groups for vis (0 == default, 1 == always visible, 2 == never visible. |
| pwatchent | -1 | cl, cheat | Entity to watch for prediction system changes. |
| pwatchvar | 0 | cl, cheat | Entity variable to watch in prediction system for changes. |
| quit | cmd | release, vconsole_set_focus | Quit the game |
| r_AirboatViewDampenDamp | 1 | sv, cl, nf, rep, cheat |  |
| r_AirboatViewDampenFreq | 7 | sv, cl, nf, rep, cheat |  |
| r_AirboatViewZHeight | 0 | sv, cl, nf, rep, cheat |  |
| r_citadel_cloak_blur_amount | 0.01 | cl, cheat | cloak |
| r_citadel_cloak_blur_factor_max_roughness | 1 | cl, cheat | cloak |
| r_citadel_cloak_blur_factor_min_roughness | 1 | cl, cheat | cloak |
| r_citadel_cloak_blur_noise_amount | 0.5 | cl, cheat | cloak |
| r_citadel_cloak_color_tint | 230 230 230 | cl, cheat | cloak |
| r_citadel_cloak_fresnel_effect | 0 | cl, cheat | cloak |
| r_citadel_cloak_intensity | 1 | cl, cheat | cloak |
| r_citadel_cloak_refract_amount | 0 | cl, cheat | cloak |
| r_citadel_cosmic_veil_fade_dist | 32 | cl, cheat | cosmic veil |
| r_citadel_glow_health_bar_debug | false | cl, cheat |  |
| r_citadel_mboit_bias | 0.000005 | cl, cheat |  |
| r_citadel_mboit_overestimation | 0.25 | cl, cheat |  |
| r_cubemap_debug_colors | 0 | cheat |  |
| r_debug_precipitation | false | cl, cheat | Show precipitation volumes |
| r_directlighting | true | cheat | Set to use direct lighting |
| r_dof_override | false | cheat |  |
| r_dof_override_far_blurry | 2000 | cheat |  |
| r_dof_override_far_crisp | 180 | cheat |  |
| r_dof_override_near_blurry | -100 | cheat |  |
| r_dof_override_near_crisp | 0 | cheat |  |
| r_dof_override_tilt_to_ground | 0.5 | cheat |  |
| r_dopixelvisibility | true | cheat |  |
| r_draw_first_tri_only | false | cheat |  |
| r_draw_instances | true | cheat |  |
| r_draw_particle_children_with_parents | -1 | cheat | Draw particle children with parents (-1=use gameinfo, 0=no, 1=yes) |
| r_drawblankworld | false | cheat | Render blank instead of the game world |
| r_drawdecals | true | cheat | Set to render decals |
| r_drawdevvisualizers | false | cl, cheat | Render dev visualizers |
| r_drawpanorama | true | cheat | Enable the rendering of panorama UI |
| r_drawparticles | true | cheat | Enable/disable particle rendering |
| r_drawropes | true | cl, cheat |  |
| r_drawskybox | true | cheat | Render the 2d skybox. |
| r_drawtracers | true | cl, cheat |  |
| r_drawtracers_firstperson | true | cl, archive release | Toggle visibility of first person weapon tracers |
| r_drawviewmodel | true | cl, cheat | Render view model |
| r_drawworld | true | cheat | Render the world. |
| r_extra_render_frames | 0 | cheat |  |
| r_fallback_texture_lod_scale | 2 | cheat | Scale factor for requested texture size (texture streaming) - used for geo that doesn't have a precomputed UV density measure |
| r_farz | -1 | cl, cheat | Override the far clipping plane. -1 means to use the value in env_fog_controller. |
| r_flashlightambient | 0 | cl, cheat |  |
| r_flashlightbacktraceoffset | 0.4 | cl, cheat |  |
| r_flashlightbrightness | 1 | cl, rep, cheat |  |
| r_flashlightconstant | 0 | cl, rep, cheat |  |
| r_flashlightfar | 1500 | cl, rep, cheat |  |
| r_flashlightfov | 53 | cl, rep, cheat |  |
| r_flashlightladderdist | 40 | cl, cheat |  |
| r_flashlightlinear | 100 | cl, rep, cheat |  |
| r_flashlightlockposition | false | cl, cheat |  |
| r_flashlightmuzzleflashfov | 120 | cl, cheat |  |
| r_flashlightnear | 4 | cl, rep, cheat |  |
| r_flashlightnearoffsetscale | 1 | cl, cheat |  |
| r_flashlightoffsetforward | 0 | cl, rep, cheat |  |
| r_flashlightoffsetright | 5 | cl, rep, cheat |  |
| r_flashlightoffsetup | -5 | cl, rep, cheat |  |
| r_flashlightquadratic | 0 | cl, rep, cheat |  |
| r_flashlightshadowatten | 0.35 | cl, cheat |  |
| r_flashlighttracedistcutoff | 128 | cl, cheat |  |
| r_flashlighttracedistwatercutoff | 80 | cl, cheat |  |
| r_flashlightvisualizetrace | false | cl, cheat |  |
| r_flush_on_pooled_ib_resize | true | release |  |
| r_force_no_present | false | cheat | Force the render device to not present frames. |
| r_force_zprepass | -1 | cheat | 0: Force z prepass off. 1: Force on. -1: Don't force |
| r_freezeparticles | false | cheat | Pause particle simulation |
| r_fullscreen_gamma | 2.2 | archive | Screen Gamma (only in fullscreen modes) |
| r_indirectlighting | true | cheat | Set to use indirect lighting |
| r_JeepViewDampenDamp | 1 | sv, cl, nf, rep, cheat |  |
| r_JeepViewDampenFreq | 7 | sv, cl, nf, rep, cheat |  |
| r_JeepViewZHeight | 10 | sv, cl, nf, rep, cheat |  |
| r_light_probe_volume_debug_colors | 0 | cheat |  |
| r_light_probe_volume_debug_grid | false | cheat | Show LPV debug grid, 0: off, 1: closest only 2 :closest and keep 3: all |
| r_light_probe_volume_debug_grid_albedo | 128 128 128 | cheat | albedo for LPV debug grid |
| r_light_probe_volume_debug_grid_bbox | true | cheat | Show LPV bounding box when debug grid is on, 0: off, 1: on |
| r_light_probe_volume_debug_grid_metalness | 0 | cheat | metalness for LPV debug grid |
| r_light_probe_volume_debug_grid_prim | 0 | cheat | 0: spheres, 1: cubes |
| r_light_probe_volume_debug_grid_roughness | 0.5 | cheat | roughness for LPV debug grid |
| r_light_probe_volume_debug_grid_samplesize | 4 | cheat | sphere radius (world) for LPV debug grid |
| r_lightmap_set | lightmaps | cheat | Lightmap set to use, only works on map load |
| r_mapextents | 16384 | cl, cheat | Set the max dimension for the map.  This determines the far clipping plane |
| r_morphing_enabled | true | cheat |  |
| r_muzzleflashbrightness | 0.4 | cl, rep, cheat |  |
| r_muzzleflashlinear | 0.05 | cl, rep, cheat |  |
| r_nearz | -1 | cl, cheat | Override the near clipping plane. -1 means use the default. |
| r_particle_max_draw_distance | 1000000 | cheat | The maximum distance that particles will render |
| r_pixelvisibility_partial | true | cheat |  |
| r_pixelvisibility_spew | false | cheat |  |
| r_render_world_node_bounds | false | cheat | Render world node bounds |
| r_rendersun | true | cheat | Render sun lighting |
| r_replay_post_effect | -1 | cl, cheat |  |
| r_shadows | true | cheat |  |
| r_showdebugoverlays | false | cheat | Set to render debug overlays |
| r_showdebugrendertarget | false | cheat | Set the debug render target to show, 0 == disable |
| r_showsceneobjectbounds | false | cheat | Show scenesystem object bounding boxes |
| r_showsunshadowdebugrendertargets | false | cheat | Set to render sun shadow render targets |
| r_showsunshadowdebugsplitvis | false | cheat | Set to render sun shadow split visibility debugger |
| r_size_cull_threshold_shadow | 0.2 | cheat | Threshold of shadow map size percentage below which objects get culled |
| r_skinning_enabled | true | cheat |  |
| r_smooth_morph_normals | true | release |  |
| r_stereo_multiview_instancing | false | cheat | Use multiview instancing for stereo rendering. |
| r_texture_lod_scale | 1 | cheat | Scale factor for requested texture size (texture streaming) |
| r_translucent | true | cheat | Enable rendering of translucent geometry |
| r_zprepass_normals | false | cheat | 0: Use normals reconstructed from depth. 1: Output correct normals in z prepass. |
| ragdoll_biped_settle_duration | 1.5 | sv, cheat |  |
| ragdoll_biped_settle_force | 0.5 | sv, cheat |  |
| ragdoll_biped_settle_lift_force | 0.2 | sv, cheat |  |
| ragdoll_biped_settle_start_time | 0.5 | sv, cheat |  |
| ragdoll_biped_settle_vertical_limit | 0.7 | sv, cheat |  |
| ragdoll_lru_debug_removal | false | sv, cl, rep, cheat |  |
| ragdoll_lru_min_age | 10 | sv, cl, rep, cheat |  |
| ragdoll_move_entity | false | sv, cl, rep, cheat |  |
| ragdoll_resolve_initial_conflict | false | sv, cl, rep, cheat |  |
| ragdoll_resolve_separation | false | sv, cl, rep, cheat |  |
| ragdoll_set_weight | cmd | sv, rep, cheat | ragdoll_set_weight |
| ragdoll_update_from_weights | false | sv, cl, rep, cheat |  |
| rangefinder | cmd | sv, cheat | Measures distance along a ray |
| rangefinder2d | cmd | sv, cheat | Measures distance along a ray, only measuring along XY plane. |
| rate | 786432 | archive user | Min bytes/sec the host can receive data |
| rcon | cmd | norecord, release | Issue an rcon command. |
| rcon_address | 0 | norecord, release, server_cant_query | Address of remote server if sending unconnected rcon commands (format x.x.x.x:p) |
| rcon_connected_clients_allow | true | replicated release | Allow clients to use rcon commands on server. |
| rcon_password | 0 | norecord, release, server_cant_query | remote console password. |
| recast_mark_overhang | true | rep, cheat | Enable/disable overhang detection |
| recast_partitioning | 0 | rep, cheat | 0 = watershed, 1 = monotone, 2 = layers |
| record | cmd | norecord, release | Record a demo. |
| reloadgame | cmd | cheat, vconsole_set_focus | Reload the most recent saved game. |
| remove_weapon | cmd | sv, cheat | Remove a weapon held by the player.  Arguments: <weapon subclass name> |
| repeat_last_console_command | cmd | release | Repeat last console command. |
| replay_death | cmd | sv, cheat | start hltv replay of last death |
| replay_debug | 0 | replicated release |  |
| replay_start | cmd | sv, cheat | Start GOTV replay: replay_start <delay> [<player name or index>] |
| replay_stop | cmd | sv | stop hltv replay |
| report_cliententitysim | false | cl, cheat | List all clientside simulations and time - will report and turn itself off. |
| report_clientthinklist | false | cl, cheat | List all clientside entities thinking and time - will report and turn itself off. |
| reset_gameconvars | cmd | cheat | Reset game convars to default values |
| reset_voice_on_input_stallout | false | user | If true, resets the input device when there was a long enough hitch between callbacks. |
| respawn_player | cmd | sv, cheat | Respawns the player from death! |
| restart | cmd | cheat, vconsole_set_focus | Poor man's restart: reload the current map from disk. |
| rr_followup_maxdist | 1800 | sv, cheat | 'then ANY' or 'then ALL' response followups will be dispatched only to characters within this distance. |
| rr_forceconcept | cmd | sv, cheat | fire a response concept directly at a given character. USAGE: rr_forceconcept <target name or index> <concept> 'criteria1:value1,criteria2:value2,...' criteria values are optional. |
| rr_reloadresponsesystems | cmd | sv, cheat | Reload all response system scripts. |
| rr_thenany_score_slop | 0 | sv, a, cheat | When computing respondents for a 'THEN ANY' rule, all rule-matching scores within this much of the best score will be considered. |
| run_perftest | cmd | cheat, norecord | Execute perftest.cfg |
| save_animgraph_recording | cmd | sv, cheat | Saves all active animgraph recordings to disk  Arguments: automaticallyOpenInAnimgraphEditor |
| save_maxarray_spew | 10 | sv, release | Max number of array entries to spew when using SaveRestoreIO spewing. |
| say | cmd | sv | Display player message |
| say_chat | cmd | cl, release | Opens chat menu to chat with everyone |
| say_chat_team | cmd | cl, release | Opens chat menu to chat with Allies |
| say_team | cmd | sv | Display player message to team |
| sc_aggregate_indirect_draw_compaction | true | release | Use multidrawindirect...count if the driver/hardware supports it |
| sc_aggregate_indirect_draw_compaction_threshold | 8 | release | Threshold of indirect draws when we will do compaction |
| sc_check_world | false | cheat |  |
| sc_disable_culling_boxes | false | cheat |  |
| sc_disable_procedural_layer_rendering | false | cheat |  |
| sc_disable_shadow_fastpath | false | cheat |  |
| sc_disable_shadow_materials | false | cheat |  |
| sc_disable_spotlight_shadows | false | cheat |  |
| sc_disable_world_materials | false | cheat |  |
| sc_disableThreading | false | cheat |  |
| sc_dump_lists | false | cheat |  |
| sc_dumpworld | cmd | cheat | Dump a list of the objects in a sceneworld (Usage: sc_dumpworld <world_index>) |
| sc_dumpworld3d | cmd | cheat | Dump the objects in a sceneworld into a 3d geoview buffer (Usage: sc_dumpworld3d <world_index>) |
| sc_extended_stats | false | cheat |  |
| sc_fade_distance_scale_override | -1 | cheat |  |
| sc_force_lod_level | -1 | cheat |  |
| sc_force_materials_batchable | false | cheat |  |
| sc_force_translation_in_projection | false | cheat | If enabled, the camera's translation will be included in the projection matrix. |
| sc_listworlds | cmd | cheat | List all the active sceneworlds |
| sc_only_render_opaque | false | cheat |  |
| sc_only_render_shadowcasters | false | cheat |  |
| sc_reject_all_objects | false | cheat |  |
| sc_screen_size_lod_scale_override | -1 | cheat |  |
| sc_setclassflags | cmd | cheat | Low level command to set the flags byte associated with an object class. sc_SetClassFlags <classname> <value> |
| sc_showclasses | cmd | cheat | List the object class names known by scenesystem |
| sc_skip_traversal | false | cheat |  |
| scale_function_dump | cmd | sv, cheat | Print out all scale functions. |
| scene_playvcd | cmd | sv, cheat | Play the given VCD as an instanced scripted scene. |
| scene_showfaceto | false | sv, a, cheat | When playing back, show the directions of faceto events. |
| scene_showmoveto | false | sv, a | When moving, show the end location. |
| screenmessage_show | -1 | cheat | Enable display of console messages on screen. 1 = Enabled, 0 = Disabled, -1 = Enabled if vgui is not present |
| script_add_debug_filter | cmd | sv, cheat | Add a filter to the game debug overlay |
| script_add_watch | cmd | sv, cheat | Add a watch to the game debug overlay |
| script_add_watch_pattern | cmd | sv, cheat | Add a watch to the game debug overlay |
| script_attach_debugger | cmd | sv, cheat | Connect the vscript VM to the script debugger |
| script_clear_watches | cmd | sv, cheat | Clear all watches from the game debug overlay |
| script_debug | cmd | sv, cheat | Toggle the in-game script debug features |
| script_dump_all | cmd | sv, cheat | Dump the state of the VM to the console |
| script_find | cmd | sv, cheat | Find a key in the VM |
| script_help | cmd | sv, cheat | Output help for script functions |
| script_reload | cmd | sv, cheat | Reload scripts |
| script_reload_code | cmd | sv, cheat | Execute a vscript file, replacing existing functions with the functions in the run script |
| script_reload_entity_code | cmd | sv, cheat | Execute all of this entity's VScripts, replacing existing functions with the functions in the run scripts |
| script_remove_debug_filter | cmd | sv, cheat | Remove a filter from the game debug overlay |
| script_remove_watch | cmd | sv, cheat | Remove a watch from the game debug overlay |
| script_remove_watch_pattern | cmd | sv, cheat | Remove a watch from the game debug overlay |
| script_resurrect_unreachable | cmd | sv, cheat | Use the garbage collector to track down reference cycles |
| script_trace_disable | cmd | sv, cheat | Turn off a particular trace output by file or function name |
| script_trace_disable_all | cmd | sv, cheat | Turn off all trace output |
| script_trace_disable_key | cmd | sv, cheat | Turn off a particular trace output by table/instance |
| script_trace_enable | cmd | sv, cheat | Turn on a particular trace output by file or function name |
| script_trace_enable_all | cmd | sv, cheat | Turn on all trace output |
| script_trace_enable_key | cmd | sv, cheat | Turn on a particular trace output by table/instance |
| sdr | cmd | release | An old command that has been renamed to 'net_option' |
| sensitivity | 1.25 | cl, archive user, per_user | Mouse sensitivity. |
| servercfgfile | server.cfg | sv, release |  |
| setang | cmd | sv, cheat | Snap player eyes to specified pitch yaw <roll:optional> (must have sv_cheats). |
| setang_exact | cmd | sv, cheat | Snap player eyes and orientation to specified pitch yaw <roll:optional> (must have sv_cheats). |
| setinfo | cmd | clientcmd_can_execute | Adds a new user info value |
| setmodel | cmd | sv, cheat | Changes's player's model |
| setpause | cmd | release | Set the pause state of the server. |
| setpos | cmd | sv, cheat | Move player to specified origin (must have sv_cheats). |
| setpos_exact | cmd | sv, cheat | Move player to an exact specified origin (must have sv_cheats). |
| setpos_player | cmd | sv, cheat | Move specified player to specified origin (must have sv_cheats). |
| shake | cmd | sv, cheat | Shake the screen. |
| shake_stop | cmd | cl, cheat | Stops all active screen shakes. |
| shake_testpunch | cmd | cl, cheat | Test a punch-style screen shake. |
| shatterglass_break | cmd | sv, cheat |  |
| shatterglass_cleanup | true | sv, cl, rep, cheat |  |
| shatterglass_cleanup_max | 200 | sv, cl, rep, cheat |  |
| shatterglass_debug | false | sv, cl, rep, cheat |  |
| shatterglass_hit_tolerance | 2 | sv, cl, rep, cheat |  |
| shatterglass_restore | cmd | sv, cheat |  |
| shatterglass_shard_lifetime | 15 | sv, cl, rep, cheat |  |
| show_steam_id | cmd | cl, release | Prints out the local user's Steam ID. Handy for getting account ID for a player |
| show_visibility_boxes | false | cl, cheat | Enable or Disable debug display of visibility boxes |
| showconsole | cmd | norecord, release | Show the console. |
| showtriggers | cmd | sv, cheat | Enable or Disable showing trigger entities |
| showtriggers_toggle | cmd | sv, cheat | Displays the movement bounding box for the triggers in orange.  Some entites will also display entity specific overlays.  Arguments:    {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| silence_dsp | false | cheat | When on, silences all DSP mixes. |
| sk_autoaim_mode | 1 | sv, cl, a, rep |  |
| skel_constraints_enable | true | rep, cheat |  |
| skeleton_instance_scaleset_enable | true | sv, cl, rep, cheat |  |
| skeleton_instance_smear_boneflags | false | sv, cheat | Smear boneflags across the model.  Costs computation, but tests to make sure your bone flags are consistent. |
| skill | 1 | sv, cl, a, rep, per_user | Game skill level. |
| snd_arrangement_start | cmd | cheat | Starts the specified arrangement. |
| snd_autodetect_latency | true | archive |  |
| snd_break_on_start_soundevent | 0 | sv, cl, rep, cheat | Use to debug break on any soundevent that is started matching this name |
| snd_cast | cmd | cheat | Casts a ray and starts a sound event where the ray hits. The sound event will retrigger periodically if cl_snd_cast_retrigger is set. The sound event will clear previous snd_cast events if cl_snd_cast_clear is set. Usage: snd_cast <eventname> [<retrigger time>] [<max distance>]. Arguments that are specified will become defaults for the remainder of the session. |
| snd_disable_mixer_duck | false | cheat |  |
| snd_disable_mixer_solo | false | cheat |  |
| snd_dsp_distance_max | 2000 | cheat |  |
| snd_dsp_distance_min | 20 | cheat |  |
| snd_duckerattacktime | 0.5 | archive |  |
| snd_duckerreleasetime | 2.5 | archive |  |
| snd_duckerthreshold | 0.15 | archive |  |
| snd_ducktovolume | 0.55 | archive |  |
| snd_envelope_rate | 100 | cheat |  |
| snd_filter | 0 | cheat |  |
| snd_foliage_db_loss | 4 | sv, cheat | foliage dB loss per 1200 units |
| snd_gain | 1 | archive |  |
| snd_gain_max | 1 | cheat |  |
| snd_gain_min | 0.01 | cheat |  |
| snd_gamevoicevolume | 1 | archive | Game v.o. volume |
| snd_gamevolume | 1 | archive | Game volume |
| snd_get_physics_surface_properties | cmd | cheat | Get physics surface properties for all the materials. |
| snd_group_cluster_debug | false | rep, cheat |  |
| snd_group_priority_debug | false | rep, cheat |  |
| snd_group_priority_max_tolerance | 0.05 | rep, cheat |  |
| snd_list | 0 | cheat |  |
| snd_log_empty_event_entities | false | cl, cheat | Logs the sound event entities that have empty names. |
| snd_mixahead | 0.001 | archive |  |
| snd_mixer_master_dsp | 1 | cheat |  |
| snd_mixer_master_level | 1 | cheat |  |
| snd_musicvolume | 1 | archive | Music volume |
| snd_mute_losefocus | true | archive |  |
| snd_new_visualize | false | sv, cheat | Displays soundevent name played at it's 3d position |
| snd_occlusion_bounces | 1 | rep, cheat |  |
| snd_occlusion_debug | false | sv, cl, rep, cheat |  |
| snd_occlusion_min_wall_thickness | 4 | rep, cheat |  |
| snd_occlusion_rays | 4 | rep, cheat |  |
| snd_op_test_convar | 720 | cheat |  |
| snd_opvar_set_point_debug | false | sv, cl, rep, cheat |  |
| snd_print_activetracks | cmd | cheat | List all active tracks |
| snd_print_arrangements | cmd | cheat | List all available sequence arrangments |
| snd_print_samplers | cmd | cheat | List all available samplers |
| snd_print_sequences | cmd | cheat | List all available midi sequences |
| snd_rear_stereo_scale | 1 | rep, cheat |  |
| snd_refdb | 60 | cheat | Reference dB at snd_refdist |
| snd_refdist | 36 | cheat | Reference distance for snd_refdb |
| snd_report_verbose_error | false | cheat | If set to 1, report more error found when playing sounds. |
| snd_samplers_play_note | cmd | cheat | Play a note from a specified sampler |
| snd_samplers_stop_note | cmd | cheat | Stop a note from a specified sampler |
| snd_sequence_set_track_bpm | cmd | cheat | Sets the tempo of the specified track |
| snd_sequence_set_track_transpose | cmd | cheat | Sets the transposition of the specified track |
| snd_sequence_stop_all_tracks | cmd | cheat | Stops all currently playing sequences |
| snd_sequence_stop_track | cmd | cheat | Stops the specified track |
| snd_sequencer_show_bpm | false | cheat |  |
| snd_sequencer_show_events | false | cheat |  |
| snd_sequencer_show_quantize_queue | false | cheat |  |
| snd_set_physics_surface_properties | cmd | cheat | Set physics surface properties for materials. Usage: <heuristic #> <commit> |
| snd_setmixer | cmd | cheat | Set named Mixgroup of current mixer to mix vol, mute, solo. |
| snd_setmixlayer | cmd | cheat | Set named Mixgroup of named mix layer to mix vol, mute, solo. |
| snd_showclassname | 0 | cheat |  |
| snd_showstart | 0 | cheat |  |
| snd_sos_block_global_stack | false | cheat |  |
| snd_sos_block_stop_global_stack | true | cheat |  |
| snd_sos_calc_angle_debug | false | rep, cheat |  |
| snd_sos_compare_kv3_native_stacks | false | cheat |  |
| snd_sos_compare_operator_stacks | cmd | cheat | Compares 2 operator stacks and spews any errors |
| snd_sos_flush_operators | cmd | cheat | Flush and re-parse the sound operator system |
| snd_sos_get_operator_field_info | cmd | cheat | Currently gets info for a single operator field |
| snd_sos_ingame_debug | false | cheat |  |
| snd_sos_list_operator_updates | false | cheat |  |
| snd_sos_opvar_debug | false | cheat |  |
| snd_sos_pause_soundevent | cmd | cheat | Pause the specified soundevent in the list |
| snd_sos_pause_system | false | cheat |  |
| snd_sos_print_addfield_dupes | false | cheat |  |
| snd_sos_print_class_sizes | cmd | cheat | Prints the sizes of relevant sos classes. |
| snd_sos_print_field_name_strings | cmd | cheat | Prints a list of currently cached field name strings |
| snd_sos_print_field_references | false | cheat |  |
| snd_sos_print_fps | false | cheat |  |
| snd_sos_print_full_field_info | false | cheat |  |
| snd_sos_print_groups | cmd | cheat | Prints the current state of the groups system |
| snd_sos_print_operator_stack | cmd | cheat | Prints a master list of currently exposed variables |
| snd_sos_print_operator_stack_operator | cmd | cheat | Prints an operator from a stack |
| snd_sos_print_operator_stacks | cmd | cheat | Prints a list of currently available stacks |
| snd_sos_print_operators | cmd | cheat | Prints a list of currently available operators |
| snd_sos_print_stack_exec_list | cmd | cheat | Prints the current stack execution list |
| snd_sos_print_strings | cmd | cheat | Prints a list of currently cached strings |
| snd_sos_print_table_arrays | false | cheat |  |
| snd_sos_print_tool_properties | cmd | cheat | Prints the current state of tool properties. |
| snd_sos_resolve_execute_operator | cmd | cheat | Resolve the inputs and execute one specified operator from a specified stack |
| snd_sos_set_operator_field | cmd | cheat | Currently sets a single float operator field |
| snd_sos_set_operator_field_by_guid | cmd | cheat | Currently sets a single float operator field |
| snd_sos_show_block_debug | false | cheat | Spew data about the list of block entries. |
| snd_sos_show_operator_event_and_stack | true | cheat |  |
| snd_sos_show_operator_event_filter | 0 | cheat |  |
| snd_sos_show_operator_field_filter | 0 | cheat |  |
| snd_sos_show_operator_init | false | cheat |  |
| snd_sos_show_operator_not_executing | true | cheat |  |
| snd_sos_show_operator_operator_filter | 0 | cheat |  |
| snd_sos_show_operator_pause_entry | false | cheat |  |
| snd_sos_show_operator_shutdown | false | cheat |  |
| snd_sos_show_operator_stop_entry | false | cheat |  |
| snd_sos_show_operator_updates | false | cheat |  |
| snd_sos_show_opvar_updates | false | cheat |  |
| snd_sos_show_opvar_updates_filter | 0 | cheat |  |
| snd_sos_show_queuetotrack | false | cheat |  |
| snd_sos_show_soundevent_param_overwrite | false | cheat |  |
| snd_sos_show_soundevent_start | false | cheat |  |
| snd_sos_soundevent_filter | 0 | cheat |  |
| snd_sos_soundevent_profile | cmd | cheat | Dump a record of current soundevents and profile data |
| snd_sos_start_soundevent | cmd | cheat | Starts a specified soundevent |
| snd_sos_start_soundevent_at_pos | cmd | cheat | Starts a specified soundevent at the given position |
| snd_sos_start_stack | cmd | cheat | Starts a specified stack via an empty soundevent |
| snd_sos_stop_all_soundevents | cmd | cheat | Stops all soundevents currently on the execution list |
| snd_sos_stop_soundevent_guid | cmd | cheat | Stops a specified soundevent |
| snd_sos_stop_soundevent_index | cmd | cheat | Stops a specified soundevent |
| snd_sos_test_soundmessage | cmd | cheat | test |
| snd_sos_unpause_soundevent | cmd | cheat | UnPause the first soundevent in the list |
| snd_sound_areas_debug | false | cl, rep, cheat |  |
| snd_sound_areas_debug_interval | 0.2 | cl, rep, cheat |  |
| snd_soundmixer_set_trigger_factor | cmd | cheat | Set named mix layer / mix group, trigger amount. |
| snd_soundmixer_setmixlayer_amount | cmd | cheat | Set named mix layer mix amount. |
| snd_soundmixer_update_maximum_frame_rate | 0 | cheat |  |
| snd_spatialize_lerp | 0 | archive release |  |
| snd_steamaudio_baked_data_stats | cmd | cheat | Display baked data stats for the current mod. |
| snd_steamaudio_enable_pathing | false | cheat | This variable is checked by soundstack to globally enabling pathing for audio processing. |
| snd_steamaudio_enable_perspective_correction | false | archive release | Enable perspective correction for 3D audio. |
| snd_steamaudio_enable_reverb | 0 | release | Enable Steam Audio Reverb processor. |
| snd_steamaudio_enable_spatial_blend_fix | cmd | cheat | Toggles the speculative fix for low-frequency issues when using spatial blend. |
| snd_steamaudio_export_scene | cmd | cheat | Exports scene currently used by Steam Audio as a phononscene file. |
| snd_steamaudio_halton_sequence | cmd | cheat | Generate Halton Sequence for a given order and number of samples. |
| snd_steamaudio_ir_duration | 1 | cheat | The time delay between a sound being emitted and the last audible reflection in Steam Audio. |
| snd_steamaudio_max_convolution_sources | 4 | cheat | The maximum number of simultaneous sources that can be modeled by Steam Audio. |
| snd_steamaudio_max_occlusion_samples | 64 | cheat | The maximum number of rays that can be traced for volumetric occlusion by Steam Audio. |
| snd_steamaudio_num_bounces | 128 | cheat | The maximum number of times any ray can bounce when using Steam Audio. |
| snd_steamaudio_num_diffuse_samples | 2048 | cheat | The number of directions considered for ray bounce by Steam Audio. |
| snd_steamaudio_num_rays | 65536 | cheat | The number of rays to trace for reflection modeling by Steam Audio. |
| snd_steamaudio_num_threads | 2 | cheat | Sets the number of threads used for realtime reflection by Steam Audio. |
| snd_steamaudio_pathing_order | 1 | cheat | The amount of directional detail in the simulated by Steam Audio. |
| snd_steamaudio_pathing_order_rendering | 1 | cheat | The amount of directional detail in the rendered audio by Steam Audio. |
| snd_steamaudio_reverb_level_db | -3 | release | Adjust overall volume (dB) of the output from Steam Audio Reverb processor. |
| snd_steamaudio_source_pathing_debug | false | archive | Enable path visualization for steam_audio_source operator. |
| snd_toolvolume | 1 | archive | Volume of sounds in tools (e.g. Hammer, SFM) |
| snd_use_baked_occlusion | 0 | rep, cheat, release |  |
| snd_vmidi_flush | cmd | cheat | Purge and reload all vmidi data and files. |
| snd_vmix_override_mix_decay_time | -1 | cheat | If set > 0, overrides how long the decay time is on all mix graphs (in seconds). |
| snd_vmix_show_input_updates | false | cheat | If set to 1, show all incoming updates to vmix inputs. |
| snd_voipvolume | 1 | archive | Voice volume |
| sound_device_override | 0 | archive release | ID of the sound device to use |
| soundinfo | cmd | release | Describe the current sound device with an active voice list. |
| soundscape_debug | false | sv, cheat | When on, draws lines to all env_soundscape entities. Green lines show the active soundscape, red lines show soundscapes that aren't in range, and white lines show soundscapes that are in range, but not the active soundscape. |
| soundscape_dumpclient | cmd | cl, cheat | Dumps the client's soundscape data. |
| soundscape_fadetime | 3 | cl, cheat | Time to crossfade sound effects between soundscapes |
| soundscape_radius_debug | false | cl, cheat | Prints current volume of radius sounds |
| spawn_group_activate | cmd | sv, cheat | Activate specified spawngroup. |
| spawn_group_load | cmd | sv, cheat | Load named spawn group. |
| spawn_group_unload | cmd | sv, cheat | Unload named spawn group. |
| speaker_config | 0 | archive |  |
| spec_autodirector | true | cl, clientcmd_can_execute | Auto-director chooses best view modes while spectating |
| spec_centerchasecam | false | cl, archive | Looks at the target player's center, instead of his eye position, in chase came mode |
| spec_chase | cmd | cl, release | Changes the spectate mode to chase |
| spec_goto | cmd | cl, release | Changes the spectate mode to roaming and go to the location |
| spec_in_eye | cmd | cl, release | Changes the spectate mode to in-eye |
| spec_mode | cmd | cl, clientcmd_can_execute | Set spectator mode |
| spec_next | cmd | cl, clientcmd_can_execute | Spectate next player |
| spec_player | cmd | cl, clientcmd_can_execute | Spectate a player by name or slot |
| spec_pos | cmd | cl, cheat | dump position and angles to the console |
| spec_prev | cmd | cl, clientcmd_can_execute | Spectate previous player |
| spec_replay_autostart | true | cl, archive | Auto-start Killer Replay when available |
| spec_replay_bot | false | sv, release | Enable Spectator Hltv Replay when killed by bot |
| spec_replay_enable | 0 | replicated release | Enable Killer Replay, requires hltv server running (0:off, 1:default, 2:force) |
| spec_replay_leadup_time | 5.3438 | replicated release | Replay time in seconds before the highlighted event |
| spec_replay_message_time | 9.5 | replicated release | How long to show the message about Killer Replay after death. The best setting is a bit shorter than spec_replay_autostart_delay + spec_replay_leadup_time + spec_replay_winddown_time |
| spec_replay_on_death | false | replicated release | When > 0, sets the mode whereas players see delayed replay, and are segregated into a domain of chat and voice separate from the alive players |
| spec_replay_rate_base | 1 | replicated release | Base time scale of Killer Replay.Experimental. |
| spec_replay_rate_limit | 3 | replicated release | Minimum allowable pause between replay requests in seconds |
| spec_replay_winddown_time | 2 | sv, release | The trailing time, in seconds, of replay past the event, including fade-out |
| spec_target | cmd | cl, release | Changes the target being spectated |
| splitscreen_mode | 0 | a, cheat |  |
| startdemos | cmd | release | Play demos in demo sequence. |
| status | cmd | release | Print connection status |
| status_json | cmd | release | Print status in JSON format |
| stop | cmd | release | Finish recording demo. |
| stopdemos | cmd | release | Stop looping demos (current demo will complete). |
| stopsound | cmd | cheat |  |
| stopsoundscape | cmd | cl, cheat | Stops all soundscape processing and fades current looping sounds |
| subclass_change | cmd | sv, cheat, vconsole_fuzzy | Changes the subclass of the given entity.  Arguments:    <new_subclass> {entity_name} / {class_name} / {entity_index} / {no argument = pick what player is looking at} |
| subclass_create | cmd | sv, cheat, vconsole_fuzzy | Creates an entity of the given subclass where the player is looking. |
| surfaceprop | cmd | sv, cheat | Reports the surface properties at the cursor |
| sv_accelerate | 10 | sv, cl, nf, rep, release |  |
| sv_airaccelerate | 10 | sv, cl, nf, rep, release |  |
| sv_allchat | true | sv, nf, release | Players can receive all other players' text chat, no death restrictions |
| sv_alltalk | false | sv, nf, release | Players can hear all other players' voice communication, no team restrictions |
| sv_audio_log_participant_start_messages | false | sv, cheat | Prints when a participant sound message was sent. |
| sv_banid_enabled | true | release | Whether server supports banid command |
| sv_bounce | 0 | sv, cl, nf, rep, release | Bounce multiplier for when physically simulated objects collide with other objects. |
| sv_cheats | false | nf, replicated release | Allow cheats on server |
| sv_citadel_bebop_beam_draw_points | false | sv, cheat |  |
| sv_citadel_log_ability_use | false | sv, release |  |
| sv_clockcorrection_msecs | 60 | sv, release | The server tries to keep each player's m_nTickBase withing this many msecs of the server absolute tickcount |
| sv_cluster | 0 | release | Data center cluster this server lives in. |
| sv_cq_trim_bloat_remainder | 1 | sv, release | When trimming a bloated CQ, leave at least N more commands than the minimum |
| sv_cq_trim_bloat_space | 0 | sv, release | When trimming a bloated CQ, try to leave room for N more commands to be added.  0 will trim only what is needed to remove the immediate bloat, a very large value will reset the whole queue. |
| sv_cq_trim_catchup_remainder | 1 | sv, release | When trimming an overful CQ due to app 'catchup' request, leave at least N more commands than the minimum |
| sv_crash_sentinel_filename | 0 | sv, release | Filename of crash detection sentinel |
| sv_debug_client_not_in_pvs | false | sv, cheat | If set, draw failed client PVS checks with red box |
| sv_debug_overlays_bandwidth | 65536 | release | Broadcast server debug overlays traffic |
| sv_debug_overlays_broadcast | false | nf, cheat, release | Broadcast server debug overlays |
| sv_enable_alternate_baselines | 1 | release | Allow alternate baseline system, set to 2 for debugging spew. |
| sv_enable_delta_packing | true | release | When enabled, this allows for entity packing to use the property changes for building up the data. This is many times faster, but can be disabled for error checking. |
| sv_ent_showonlyhitbox | -1 | sv, cheat |  |
| sv_ents_write_alarm | 0 | release | Print callstack every time CNetworkGameServerBase:WriteEntityUpdate takes more than this amount of milliseconds |
| sv_friction | 4 | sv, cl, nf, rep, release | World friction. |
| sv_gameinstructor_disable | false | cl, replicated release | Force all clients to disable their game instructors. |
| sv_gameinstructor_enable | false | cl, replicated release | Force all clients to enable their game instructors. |
| sv_gravity | 800 | sv, cl, nf, rep, release | World gravity. |
| sv_hibernate_postgame_delay | 5 | release | # of seconds to wait after final client leaves before hibernating. |
| sv_hibernate_when_empty | true | release | Puts the server into extremely low CPU usage mode when no clients connected |
| sv_hoststate_quit_syscall | false | release | When enabled, game server will quit immediately via syscall instead of running host states shutdown sequence |
| sv_infinite_ammo | 0 | sv, cl, rep, cheat, release | Player's active weapon will never run out of ammo |
| sv_ladder_slack_z_mult | 0.026 | sv, cl, rep, cheat | Difference in Z increases toward the middle of the slack ladder. |
| sv_lagcompensationforcerestore | true | sv, cheat | Don't test validity of a lag comp restore, just do it. |
| sv_lan | false | release | Server is a lan server ( no heartbeat, no authentication, no non-class C addresses ) |
| sv_late_commands_allowed | 5 | sv, release | Allow N late commands to run at 0 timescale prior to running an on-time command. Negative values for network round trip based calculation with a hard cap of the of absolute value |
| sv_lightquery_debug | false | sv, cheat |  |
| sv_log_onefile | false | archive release | Log server information to only one file. |
| sv_logbans | false | archive release | Log server bans in the server logs. |
| sv_logblocks | false | release | If true when log when a query is blocked (can cause very large log files) |
| sv_logecho | true | archive release | Echo log information to the console. |
| sv_logfile | false | archive release | Log server information in the log file. |
| sv_logflush | false | archive release | Flush the log file to disk on each write (slow). |
| sv_logsdir | logs | archive release | Folder in the game directory where server logs will be stored. |
| sv_matchmaking_enabled | false | sv, rep, release | Register with the GC for matchmaking |
| sv_matchperfstats_send_to_steam | true | sv, release | Set to false to disable sending match perf stats to steam |
| sv_max_queries_sec | 3 | release | Maximum queries per second to respond to from a single IP address. |
| sv_max_queries_sec_global | 60 | release | Maximum queries per second to respond to from anywhere. |
| sv_max_queries_window | 30 | release | Window over which to average queries per second averages. |
| sv_maxrate | 0 | replicated release | Max bandwidth rate allowed on server, 0 == unlimited |
| sv_maxspeed | 320 | sv, cl, nf, rep, release |  |
| sv_maxunlag | 0.2 | sv, release | Maximum lag compensation in seconds |
| sv_maxupdaterate | 60 | sv, cl, rep, release | Maximum updates per second that the server will allow |
| sv_maxvelocity | 3500 | sv, cl, rep, release | Maximum speed any ballistically moving object is allowed to attain per axis. |
| sv_memlimit | 0 | cheat, release | If set, whenever a game ends, if the total memory used by the server is greater than this # of megabytes, the server will exit. |
| sv_merge_changes_after_tick_with_calcdelta | 1 | release | This fixes bugs where pure calcdelta is used due to recipient changing but it doesn't pick up a field change where the value was changed back to same value as the from snapshot even though the destination fields change list does note the change. Set to 2 to spew any changes merged in by this fix. |
| sv_metaduplication | cmd | cheat | Check serializer meta for duplication, add verbose to command for full spew |
| sv_minrate | 98304 | replicated release | Min bandwidth rate allowed on server, 0 == unlimited |
| sv_minupdaterate | 10 | sv, cl, rep, release | Minimum updates per second that the server will allow |
| sv_networkvar_perfieldtracking | true | release | Track individual field offset changes, rather than a single dirty flag for the whole entity. |
| sv_networkvar_validate | false | release | Validate each StateChanged against known offsets. |
| sv_noclipaccelerate | 5 | sv, cl, a, nf, rep |  |
| sv_noclipduringpause | false | sv, cl, rep, cheat | If cheats are enabled, then you can noclip with the game paused (for doing screenshots, etc.). |
| sv_noclipfriction | 4 | sv, cl, a, nf, rep | Friction during noclip move. |
| sv_noclipspeed | 1200 | sv, cl, a, nf, rep |  |
| sv_packstats | cmd | release | Show entity packing stats, pass 'clear' as argument to reset counts. |
| sv_parallel_checktransmit | 2 | sv, release | Set to 1 to use threaded checkentities for transmit/pvs on listen servers, 2 for dedicated servers. |
| sv_parallel_checktransmit | 0 | sv | Set to 1 to use threaded checkentities for transmit/pvs on listen servers, 2 for dedicated servers. |
| sv_parallel_packentities | 2 | release | Set to 1 to use threaded snapshot sending on listen servers, 2 for dedicated servers. |
| sv_parallel_sendsnapshot | 2 | release | 0: run all send jobs on main thread; 1: send jobs run asynchronously (except on dedicated server); 2: send jobs asynchronously; 3: send jobs run in parallel but block to not overlap the next tick; 4: main server clients' send jobs run in parallel, then HLTV server jobs; this approximately matches pre-async profile for a single HLTV server configuration |
| sv_password | 0 | prot, nf, norecord, release | Server password for entry into multiplayer games |
| sv_pausable | 0 | release | Is the server pausable. |
| sv_pause_on_console_open | false | archive | 1 = Pause the game when pressing ~ to open the console. CTRL+~ opens the console without pause. |
| sv_phys_debug_callback_entities | false | sv, cheat | Print all entities that get touch callbacks. Each entity is printed only once. |
| sv_phys_enabled | true | sv, cheat | Enable all physics simulation |
| sv_phys_sleep_enable | true | sv, cheat | Enable sleeping for dynamic physics bodies. |
| sv_phys_stop_at_collision | 0 | sv, cheat |  |
| sv_play_stats_CitadelLaneMatchup_enabled | true | sv, release | Enable / Disable Play Stat CitadelLaneMatchup. |
| sv_play_stats_CitadelLaneTrooperOrbs_enabled | true | sv, release | Enable / Disable Play Stat CitadelLaneTrooperOrbs. |
| sv_play_stats_CitadelMatch_enabled | true | sv, release | Enable / Disable Play Stat CitadelMatch. |
| sv_play_stats_CitadelPlayer_enabled | true | sv, release | Enable / Disable Play Stat CitadelPlayer. |
| sv_pure | cmd | release | Show user data. |
| sv_pure_kick_clients | true | release | If set to 1, the server will kick clients with mismatching files. Otherwise, it will issue a warning to the client. |
| sv_pure_trace | 0 | release | If set to 1, the server will print a message whenever a client is verifying a CRC for a file. |
| sv_pvs_max_distance | 0 | replicated release | if set, adds a maximum range to PVS/PAS checks |
| sv_ragdoll_lru_debug | false | sv, rep, cheat |  |
| sv_regeneration_force_on | false | sv, cheat | Cheat to test regenerative health systems |
| sv_region | -1 | release | The region of the world to report this server in. |
| sv_search_key | 0 | release |  |
| sv_setsteamaccount | cmd | release | token Set game server account token to use for logging in to a persistent game server account |
| sv_showlagcompensation | 0 | sv, cl, rep, cheat | If > 0, show lag compensated hitboxes whenever a player is lag compensated. Value is for how long. |
| sv_shutdown | cmd | release | Sets the server to shutdown when all games have completed |
| sv_skel_constraints_enable | false | rep, cheat |  |
| sv_skyname | sky_urb01 | sv, cl, a, rep | Current name of the skybox texture |
| sv_snapshot_unlimited | false | replicated release | For debugging, don't throw away old snapshots so that if you break in debugger (on remote client or server) it won't require an uncompressed update to resume.  You may run out of memory of course... |
| sv_soundscape_printdebuginfo | cmd | sv, cheat | print soundscapes |
| sv_specaccelerate | 5 | sv, cl, a, nf, rep |  |
| sv_specnoclip | true | sv, cl, a, nf, rep |  |
| sv_specspeed | 1200 | sv, cl, a, nf, rep |  |
| sv_spewmeta | cmd | cheat | Spew serializer meta |
| sv_steamauth_enforce | 2 | release | By default, player must maintain a reliable connection to Steam servers. When player Steam session drops, enforce it: 2 = instantly kick, 1 = kick at next spawn, 0 = do not kick. |
| sv_steamgroup | 0 | nf, release | The ID of the steam group that this server belongs to. You can find your group's ID on the admin profile page in the steam community. |
| sv_steamgroup_exclusive | false | release | If set, only members of Steam group will be able to join the server when it's empty, public people will be able to join the server only if it has players. |
| sv_stopspeed | 100 | sv, cl, nf, rep, release | Minimum stopping speed when on ground. |
| sv_stressbots | false | release | If set to 1, the server calculates data and fills packets to bots. Used for perf testing. |
| sv_tags | 0 | nf, release | Server tags. Used to provide extra information to clients when they're browsing for servers. Separate tags with a comma. |
| sv_unlockedchapters | 1 | archive | Highest unlocked game chapter. |
| sv_unpause_on_console_close | false | archive | 1 = Unpause the game when pressing ~ to close the console. 0 = Leave the game paused. |
| sv_usercmd_custom_random_seed | false | sv, release | When enabled server will populate an additional random seed independent of the client |
| sv_usercmd_execute_warning_ms | 5 | sv, a | Emit a warning if we spend more than N ms executing user commands for a single player |
| sv_vac_webapi_auth_key | 0 | sv, release | Key for when posting to vac related webapis. |
| sv_visiblemaxplayers | -1 | release | Overrides the max players reported to prospective clients |
| sv_voicecodec | vaudio_speex | release | Specifies which voice codec DLL to use in a game. Set to the name of the DLL without the extension. |
| sv_voiceenable | true | archive nf, release |  |
| sv_watchtransmit | -2 | sv, release | Watch NetworkStateChanged info for this entity index. |
| sv_wateraccelerate | 10 | sv, cl, nf, rep, release |  |
| sv_waterfriction | 1 | sv, cl, nf, rep, release |  |
| sys_info | cmd | release | Print system information to the console |
| sys_minidumpspewlines | 2000 | release | Lines of crash dump console spew to keep. |
| team_chat_auto_join | false | cl, archive release | Auto-join Team Chat when joining a match. Will be overridden by any party settings. |
| telemetry_message | cmd | sv, cheat | Place a message in the telemetry timeline |
| telemetry_toggle_timespan | cmd | sv, cheat | Starts/stops a timespan with an ever increasing name. |
| Test_CreateEntity | cmd | sv, cheat |  |
| test_dispatcheffect | cmd | sv, cheat | Test a clientside dispatch effect.  Usage: test_dispatcheffect <effect name> <distance away> <flags> <magnitude> <scale>  Defaults are: <distance 1024> <flags 0> <magnitude 0> <scale 0> |
| Test_EHandle | cmd | sv, cheat |  |
| test_entity_blocker | cmd | sv, cheat | Test command that drops an entity blocker out in front of the player. |
| Test_ExitProcess | cmd | cheat | Test_ExitProcess <exit code> - immediately kill the process. |
| test_list_entities | cmd | sv, cheat | test-list entities |
| Test_RandomPlayerPosition | cmd | sv, cheat |  |
| think_limit | 0 | sv, cl, rep, release | Maximum think time in milliseconds, warning is printed if this is exceeded. |
| thirdperson | cmd | cl, cheat, execute_per_tick | Switch to thirdperson camera. |
| thirdperson_mayamode | cmd | cl, cheat | Switch to thirdperson Maya-like camera controls. |
| think_limit | 10 | sv, cl, rep | Maximum think time in milliseconds, warning is printed if this is exceeded. |
| timedemo | cmd | release | Play a demo and report performance info. |
| timedemoquit | cmd | release | Play a demo, report performance info, and then exit |
| toggle | cmd | norecord, release | Toggles specified convar value on and off. |
| toggleconsole | cmd | norecord, release | Show/hide the console. |
| trooper_kill_all | cmd | sv, cheat | Kills all living troopers |
| trooper_kill_non_bosses | cmd | sv, cheat | Kills all non-boss living troopers |
| tv_advertise_watchable | false | prot, nf, norecord, release | GOTV advertises the match as watchable via game UI, clients watching via UI will not need to type password |
| tv_allow_autorecording_index | -1 | sv, release | When >=0 restricts autorecording only to the specified TV index |
| tv_allow_static_shots | true | sv, release | Auto director uses fixed level cameras for shots |
| tv_autorecord | false | release | Automatically records all games as SourceTV demos. |
| tv_autoretry | true | release | Relay proxies retry connection after network timeout |
| tv_broadcast | false | release | Automatically broadcasts all games as GOTV demos through Steam. |
| tv_broadcast1 | false | release | Automatically broadcasts all games as GOTV[1] demos through Steam. |
| tv_broadcast_keyframe_interval | 3 | release | The frequency, in seconds, of sending keyframes and delta fragments to the broadcast relay server |
| tv_broadcast_keyframe_interval1 | 3 | release | The frequency, in seconds, of sending keyframes and delta fragments to the broadcast1 relay server |
| tv_broadcast_max_requests | 20 | release | Max number of broadcast http requests in flight. If there is a network issue, the requests may start piling up, degrading server performance. If more than the specified number of requests are in flight, the new requests are dropped. |
| tv_broadcast_max_requests1 | 20 | release | Max number of broadcast1 http requests in flight. If there is a network issue, the requests may start piling up, degrading server performance. If more than the specified number of requests are in flight, the new requests are dropped. |
| tv_broadcast_startup_resend_interval | 10 | release | The interval, in seconds, of re-sending startup data to the broadcast relay server (useful in case relay crashes, restarts or startup data http request fails) |
| tv_broadcast_status | cmd | release | Print out broadcast status |
| tv_broadcast_url | http | //localhost | 8080: release                          : URL of the broadcast relay |
| tv_broadcast_url1 | http | //localhost | 8080: release                          : URL of the broadcast relay1 |
| tv_chatgroupsize | 0 | release | Set the default chat group size |
| tv_chattimelimit | 0.2 | release | Limits spectators to chat only every n seconds |
| tv_citadel_auto_record | true | sv, release | If enabled, a demo will automatically be recorded for every game |
| tv_clients | cmd | release | Shows list of connected SourceTV clients. |
| tv_debug | 0 | release | SourceTV debug info. |
| tv_delay | 120 | sv, release | SourceTV broadcast delay in seconds |
| tv_delay1 | 15 | sv, release | SourceTV[instance 1] broadcast delay in seconds |
| tv_deltacache | 2 | release | Enable delta entity bit stream cache |
| tv_dispatchmode | 1 | release | Dispatch clients to relay proxies: 0=never, 1=if appropriate, 2=always |
| tv_enable | false | nf, release | Activates SourceTV on server. |
| tv_enable1 | false | nf, release | Activates SourceTV[1] on server. |
| tv_enable_delta_frames | true | release | Indicates whether or not the tv should use delta frames for storage of intermediate frames. This takes more CPU but significantly less memory. |
| tv_enable_dynamic | false | nf, release | When enabled, changes in tv_enable convars cause immediate startup or shutdown of hltv server |
| tv_include_usercommands | true | sv, release | HLTV streams will include player usercommands each tick |
| tv_listen_voice_indices | 0 | cl, user | Bitfield of playerslots to listen to voice messages from when connected to SourceTV, default is none |
| tv_listen_voice_indices_h | 0 | cl, user | High 32 bits of bitfield of playerslots to listen to voice messages from when connected to SourceTV, default is none |
| tv_maxclients | 128 | release | Maximum client number on SourceTV server. |
| tv_maxclients_relayreserved | 0 | release | This number of relay client connections are reserved for SourceTV relays. |
| tv_maxrate | 0 | release | Max SourceTV spectator bandwidth rate allowed, 0 == unlimited |
| tv_mem | cmd | release | hltv memory statistics. Use with 'ent 10' (dump entity 10 memory usage) or 'top 8' (dump top 8 memory users) or 'class' CWorld (dump CWorld class) |
| tv_name | SourceTV | release | SourceTV host name |
| tv_nochat | false | archive user | Don't receive chat messages from other SourceTV spectators |
| tv_overridemaster | false | release | Overrides the SourceTV master root address. |
| tv_password | 0 | prot, nf, norecord, release | SourceTV password for all clients of CSTV[0] |
| tv_password1 | 0 | prot, nf, norecord, release | SourceTV password for all clients of CSTV[1]. If empty, tv_password is used |
| tv_playcast_delay_prediction | true | release |  |
| tv_playcast_delay_resync | 0 | release | To alleviate intermittent network connectivity problems, this is the number of seconds to wait before actually re-syncing the stream after failure |
| tv_playcast_retry_timeout | 25 | release | In case of intermittent network problems, how long should playcast retry fragment retrieval before resorting to resync |
| tv_port | 27020 | release | Host SourceTV[0] port |
| tv_port1 | 27021 | release | Host SourceTV[1] port |
| tv_record | cmd | release | Starts SourceTV demo recording. |
| tv_record_immediate | 0 | release | tv_record starting the moment tv_record was executed, not tv_delay earlier |
| tv_relay | cmd | release | Connect to SourceTV server and relay broadcast. |
| tv_relaypassword | 0 | prot, nf, norecord, release | SourceTV password for relay proxies |
| tv_relayvoice | true | release | Relay voice data: 0=off, 1=on |
| tv_retry | cmd | release | Reconnects the SourceTV relay proxy. |
| tv_secure_bypass | false | release | Bypass secure challenge on TV port |
| tv_show_allchat | true | sv, release |  |
| tv_snapshotrate | 20 | replicated release | Snapshots broadcast per second |
| tv_snapshotrate1 | 32 | release | Snapshots broadcast per second, GOTV[1] |
| tv_status | cmd | release | Show SourceTV server status. |
| tv_stop | cmd | release | Stops the SourceTV broadcast. |
| tv_stoprecord | cmd | release | Stops SourceTV demo recording. |
| tv_timeout | 20 | release | SourceTV connection timeout in seconds. |
| tv_title | SourceTV | release | Set title for SourceTV spectator UI |
| tv_transmitall | false | replicated release | Transmit all entities (not only director view) |
| tv_window_size | 16 | release | Specifies the number of seconds worth of frames that the tv replay system should keep in memory. Increasing this greatly increases the amount of memory consumed by the TV system |
| unbind | cmd | release | Unbind a key. |
| unbindall | cmd | release | Unbind all keys. |
| unpause | cmd | release | Clear the pause state of the server. |
| vconsole_rcon_server_details | 0 | norecord, release, server_cant_query | when non-empty allows for easy vconsole connection to the dedicated server. |
| viewmodel_fov | 54 | cl, cheat |  |
| violence_ablood | true | archive | Draw alien blood |
| violence_agibs | true | archive | Show alien gib entities |
| violence_hblood | true | archive | Draw human blood |
| violence_hgibs | true | archive | Show human gib entities |
| vis_force | false | sv, cheat |  |
| vismon_poll_frequency | 0.5 | sv, cheat |  |
| vismon_trace_limit | 12 | sv, cheat |  |
| vmix_input | cmd | cheat | Set an input mix value |
| vmix_output | cmd | cheat | Dump main graph control output values |
| voice_always_sample_mic | false | archive | When enabled, open the voip audio input stream when the application launches. |
| voice_device_override | 0 | archive release | Default device used for voice capture. |
| voice_input_stallout | 0.5 | user | Time before we consider a mic stalled out and need to reset it. |
| voice_loopback | false | user |  |
| voice_loopback_no_networking | false | user |  |
| voice_modenable | true | cl, archive release, clientcmd_can_execute | Enable/disable voice in this mod. |
| voice_player_speaking_delay_threshold | 0.5 | sv, cheat |  |
| voice_threshold | -120 | cl, archive | decibel threshold for how loud the talker's input signal is before we think they are talking. |
| voice_vox | 0 | cl, archive per_user, release | Voice chat uses a vox-style always on |
| volume | 1 | archive | Sound volume |
| volume_fog_debug_volumes | false | cheat |  |
| volume_fog_dither_scale | 1 | cheat |  |
| volume_fog_enable_jitter | true | cheat |  |
| vphys2_friction_factor | 1 | cheat | Change global friction factor |
| vphys2_restitution_factor | 1 | cheat | Change global restitution factor |
| wrecking_ball_muddy | 0.8 | sv, cheat | The extent to which the Wrecker's boulder behaves 'muddy', meaning how much its jumps up are dampened |
| writekeybindings | cmd | release | Saves current key bindings to disk. |
| zoom_sensitivity_ratio | 1 | cl, archive per_user | Additional mouse sensitivity scale factor applied when FOV is zoomed in. |

## Auto execute console commands on startup

[edit | edit source]

- In the <installation path>\steamapps\common\Deadlock\game\citadel\cfg folder create a text file name it autoexec.cfg
- Put the console commands that you want to run on startup of Deadlock in the autoexec.cfg file, one console command on each line and save it
- In the Steam app right-click Deadlock in your list of games on the Library tab and select Properties...
- In the "LAUNCH OPTIONS" field enter -console -exec autoexec

## Hosting Custom Games

[edit | edit source]

- The host starts a custom game by loading into the map with map dl_midtown

- You may want to pause the game immediately after joining by pressing **P** to give other players time to join the match.
- The host finds their ID by running status

- Find a green line in the console that looks like this: [Client] steamid : [A:1:XXXXXXXXXX:XXXXX] (XXXXXXXXXXXXXXXXX) (the Xs will be replaced with numbers)
- Select the part after steamid that looks like this, including the square brackets: [A:1:XXXXXXXXXX:XXXXX]
- Right click and choose "Copy Selected Text"
- The host sends players the ID they just copied. Players can now connect to the game by opening their console and running connect [A:1:XXXXXXXXXX:XXXXX] (replace the part after connect with the ID they got from the host).
- Upon joining, players will be able to select their team and hero. To bring up this menu again, players can run changeteam 0.
- If you ever want to restart the game, the host can run changelevel dl_midtown .

### Adding Bots

[edit | edit source]

- On the main menu, before you start the game, run exec citadel_botmatch_practice_6v6 to load the bot config.

- If you're already in a game, you can perform these steps then run changelevel dl_midtown to restart the game instead of starting a new one.
- Run citadel_spawn_practice_bots false so that bots won't spawn immediately when the game starts.
- Run citadel_spawn_practice_bots_count 12 to ensure that bots fill all remaining slots (they'll be added until both teams have 6 players).
- Start the game (i.e. map street_test) and press **P** to pause the game during the pregame (as soon as you load in).

- You can use citadel_pregame_duration before starting the game to increase the duration of the pregame if you want.
- Allow all other human players to connect and select their team and hero.

- The team/hero menu can be a bit glitchy. Players can use the changeteam command instead (see table above for command description).
- Remember to choose your (the host's) own team and hero as well. This may automatically unpause the game - press **P** after selecting a team to pause again.
- After all human players have joined teams and selected heroes, the host runs citadel_spawn_practice_bots true, then presses **P** again to unpause the game. Bots should fill the remaining slots on each team.

## External links

[edit | edit source]

- List of Deadlock console commands and variables on the Valve Developer Community.