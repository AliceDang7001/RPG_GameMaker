<b>YEP_CoreEngine:</b> Yanfly Engine Plugins - Core Engine is made for RPG Maker MV. This plugin
functions primarily to fix bugs and to allow the user more control over RPG
Maker MV's various features, such as the screen resolution, font, window
colors, and more.

YEP_AutoPassiveStates: Passive states are states that are automatically active. You can think of
them as an extension of traits but with more flexibility. They will always
be there as long as the actor or enemy has auto passive state notetags.

YEP_BaseTroopEvents: For all the eventers out there who love to customize their battles through
custom event pages, you can now save yourself some time by drawing all the
event pages from a base troop event to occur in every fight. All of the
events will be present in every single battle.

YEP_BattleAICore: RPG Maker MV's default enemy AI is a bit lackluster even if you managed to
have it based completely on the rates and switches. There is no way to
control the way the enemy chooses targets by default, nor are the conditions
imposed by the default editor enough to satisfy the majority of checks. This
plugin enables you to set a priority list of conditions, actions, and the
targets selected for the enemy to go through before making a decision on how
to participate in battle.

These conditions contain all of the default editor's conditions plus more,
such as determining the parameter values of a target, whether or not a state
exists on a target, the target's elemental weakness (or resistances), and
more before deciding an action. Furthermore, you can set an AI level for the
enemies to make them more consistent in the way they go about fighting your
players or more random in the way the enemies treat the priority list, too.

YEP_BattleEngineCore: This plugin alters the various aspects of the default battle system,
allowing it to be more streamlined like most modern RPG's and less clunky
like older RPG's. This ranges from choosing what text will appear in the
battle log window at the top and how it will be displayed.

YEP_BuffsStatesCore: If you are using YEP_BattleEngineCore.js, please this plugin under
YEP_BattleEngineCore in the plugin list for the best effect.

Alter the basic mechanics behind buffs and states that aren't adjustable
within the RPG Maker editor. Such mechanics include altering the maximum
number of times buffs can stack, changing the turns remaining on buffs and
states, and the rules involved when reapplying states.

A turn indicator has been added to show the amount of turns remaining on
buffs, debuffs, and states. Buffs and debuffs will operate off the plugin
parameter settings while states can operate on individual settings if you
choose for them to have unique settings.

Furthermore, a lot of Lunatic Mode options are added with this plugin to
allow those with JavaScript proficiency maximum control with states and any
unique effects that follow.

YEP_ElementCore: Elemental control in RPG Maker MV is pretty lacking. The calculation of how
multiple elements are handled aren't very clear nor are they too intuitive
when it comes to certain aspects. This plugin also gives way to skills and
items having more than one element, battlers being able to absorb, reflect,
amplify elemental damage, and more!

* Note: If you are using the Battle Engine Core, place this plugin under the
Battle Engine Core in the plugin list for additional features.

* Note: If you are using the Damage Core, place this plugin underneath the
Damage Core plugin in the list for maximum compatibility.

YEP_EquipCore: This plugin alters various aspects regarding equipment handling.

YEP_EventChasePlayer: This plugin allows you to make events that will chase the player or flee
from the player when the player enters within range of the event or when the
event sees the player.

YEP_FpsSynchOption: RPG Maker MV is constructed in a way where each update to its engine is done
once per frame update. While this is normally fine, as many players view the
game through 60 fps, some players experience the game differently as their
hardware may run at higher than 60 fps.

When RPG Maker MV version 1.1.0 is implemented, it implemented Galenmereth's
fluid timestep, which forces the game to always play as if it is 60 fps. In
practice, this is great for everybody because players that experience more
60 fps will be able to play the game as if it was 60 fps.

However, there comes a problem when a player's hardware isn't strong enough
to support RPG Maker MV natively at 60 fps (such as the case with older
computers, or weaker mobile devices) or if the player is using video
recording software that goes below 60 fps. The game will appear laggy and
jumping without good response rates from input commands or possibly even
make the player miss out on certain visual frame updates.

This plugin places a setting in the Options menu to enable or disable the
fluid timestep addition and utilize the former RPG Maker MV engine updating
function. This way, players will have the option of using fluid timesteps or
opting to not use it instead of forcing it on everybody who may not be able
to handle it.

YEP_ItemCore: This plugin makes a couple of main changes to your game and the way items
are handled to allow a base core for future plugins.

1. Independent Items
If you choose to have maximum limit on your items, weapons, and/or armors,
those items will become independent and have their own individual stats and
whatnot. Independent items are capable of being upgraded, altered, modified,
etc. and retain those changed properties independent of other items of the
same type. Items without a maximum limit (aka 0), will continue working as
they normally did in RPG Maker MV.

2. New Scene_Item
The item scene has been revamped to look a little bit different. With the
new layout, the item list is no longer two columns, but one. Added are a few
more windows, such as the item status window (which displays basic item
information), an item information window (which shows information applied to
the item via upgrades, etc.), and an item action window, which appears when
you select an item and it will ask you if you wish to Use the item or any
action added via plugins (such as upgrading the item). If you wish to not
use this revamp, you can disable it from the parameters.

3. Random Variance
Newly acquired items that aren't from shop can be given randomized stats to
a small degree for items that are independent. Items can be above the stock
value or below the stock value by the variance value. If you wish for an
item to not have a variance value, you can use a notetag to set the variance
value to 0. If you wish for all of your items to not have a variance value,
you can set the parameter to 0.

Note: During battle test, independent items are disabled.

YEP_KeyboardConfig: This plugin allows players to change their keyboard configuration from the
in-game Options menu provided that they're using a computer to play the
game and not from a mobile device. The "Keyboard Config" option will send
the player to a different screen where they can assign actions to each of
the allowed keys on the keyboard.

Certain measures are made to prevent the player from locking himself or
herself in the configuration screen. These measures are that the Enter keys
and arrow keys cannot be changed. Almost every other key is capable of being
changed to something of the player's liking.

Note: If you are using Button Common Events, place this plugin beneath
Button Common Events in the plugin parameter list.

YEP_LevelUpGrowthEffects: This plugin lets you create items that allow actor growth upon leveling up
due to the actor, the equipment worn, class, learned skills, or any states
applied to the actor upon leveling up. Growth options include increasing
basic parameters, learning new skills, turning switches on/off, full
recovery, and for those experienced with JavaScript, any kind of custom
effect that can be done using code.

YEP_MainMenuManager: For those who wish to alter the various aspects of the main menu commands
without needing to touch the source code can use this plugin to do so.
Although this plugin mostly ports the menu creation process to the Plugin
Manager parameters, it allows for a cleaner way to handle the menu command
management process.

YEP_MessageCore: While RPG Maker MV Ace certainly improved the message system a whole lot, it
wouldn't hurt to add in a few more features, such as name windows,
converting textcodes to write out the icons and/or names of items, weapons,
armours, and* more in quicker fashion. This script also gives the developer
the ability to adjust the size of the message window during the game, give
it a separate font, and to give the player a text fast-forward feature.

YEP_MoveRouteCore: RPG Maker MV gives us a lot of various commands to use for our Move Routes.
However, it still imposes a lot of limitations on the system for what else
could still be potentially useful for move route commands. This plugin will
provide additional methods to construct move routes for your events and
allow you to streamline the move route creation process.

YEP_PatchNotes: This plugin grants your players the ability to access Patch Notes from the
game itself. Being able to tell your players what you've changed from inside
the game can make all the difference in the player experience. This plugin
lets players access Patch Notes from the title screen, the main menu, or
from a Plugin Command ran inside the game.

YEP_PictureSpritesheets: In RPG Maker 2003, pictures had the ability to load spritesheets and display
certain frames from them at the issue of a command. Ever since then, later
iterations of RPG Maker lacked the feature. This plugin will bring back that
old feature and give you access to use spritesheets as pictures once more
with complete frame control.

YEP_QuestJournal: A quest journal is a very important tool provided by game developers for the
players. It lists various quests, missions, and objectives that the player
can pursue in order to progress further into the game. This can be helpful
in reminding the player what needs to be done in the event the player can
forget what things there are to do in a vast and large RPG world.

This plugin places a quest journal system into your RPG Maker MV game. You
can set up how the quest journal appears, move its windows around and/or
reshape them to fit your game. There are 100 quest slots provided by this
plugin (more can be obtained through extension plugins) and each one of them
requires your attention in constructing individually.

You can adjust the quest's title, display a difficulty level, remind the
player who the quest is from, where that quest is from, various dynamic
descriptions explaining the quest, a list of objectives to make, a list of
rewards that will be given to the player once the quest is complete, and any
subtext footnotes you may wish to insert into each quest.

---

Keep in mind that while this plugin does enable a quest journal system into
your game, this plugin will NOT automate it. If you have a quest enabled, it
is still up to you to add the quest properly into the journal, set its many
objectives, when the other objectives appear, what the rewards are, and then
giving out the rewards yourself manually. The purpose of this plugin is to
simply serve as a visual record for your player to see what quests have been
handed down to him or her.

YEP_RegionEvents: There are 255 Regions you can mark on your map. You can set it so that when
players step on those specific Regions, a Common Event will play each time
they step on it. To do so, bind a Common Event's ID to the Region number in
this plugin's parameters. It will make it so that any tile with that very
specific Region ID to trigger an on-Player Touch event using the Common
Event ID that you have marked for it.

Keep in mind that if any common event occurs during a touch input, it will
clear the touch input as intended by the game engine.

YEP_RegionRestrictions: Not everybody wants NPC's to travel all over the place. With this plugin,
you can set NPC's to be unable to move pass tiles marked by a specified
Region ID. Simply draw out the area you want to enclose NPC's in on and
they'll be unable to move past it unless they have Through on. Likewise,
there are regions that you can prevent the player from moving onto, too!

A new change from the RPG Maker VX Ace version is that now there exist
Regions that can allow players and events to always travel through.

YEP_SaveCore: This plugin provides a new save interface for the player. Along with a new
interface, the player can also load and delete saves straight from the menu
itself. This will in turn make the save command from the Main Menu always
available, but the save option within the new save menu will be enabled
depending on whether or not it is allowed or disallowed. From the interface,
the player is given more information regarding the save file including the
the location the player saved at, the amount of gold available, and any
variables that you want to show the player as well.

YEP_SaveEventLocations: Normally in RPG Maker MV, leaving a map and returning to it will reset the
map positions of all the events. For certain types of maps, such as puzzles,
you would want the map to retain their locations.

YEP_ScriptCallPluginCmd: Have you ever came across the odd situation where you wanted to use a
Plugin Command during a script call or Lunatic Mode code? This plugin will
help facilitate the process in doing so by creating a new function for you
to use in JavaScript that will transcribe the Plugin Command string and run
it during a script call.

YEP_SkillCore: Skills in RPG's consist of three main components: Costs, Damage, and
Effects. Although not all components are required for a skill, they
certainly make up a good chunk of it. Damage will be handled by another
plugin, but this plugin will provide a core handling for skill costs and
skill effects.

This plugin also includes the ability for battlers to swap their HP, MP,
and/or TP gauges for something different if it would fit the character
better (for example, some classes don't use MP and/or TP).

YEP_VictoryAftermath: This plugin swaps out the victory messages from the default battle system in
favor of more informative windows to display. Adjust the parameters to
change the settings to fit your game.

YEP_X_ActSeqPack1: The Action Sequence Pack 1 plugin is an extension plugin for Yanfly Engine
Plugins' Battle Engine Core. This extension plugin will not work without the
main plugin.

This extension plugin contains the more basic functions used for customized
action sequences on a technical scale. Here, you are able to change switches,
operate variables, add states, change damage rates, and more.

YEP_X_ActSeqPack2: The Action Sequence Pack 2 plugin is an extension plugin for Yanfly Engine
Plugins' Battle Engine Core. This extension plugin will not work without the
main plugin.

This extension plugin contains the more basic functions used for customized
action sequences on a visual scale. This plugin focuses on making battlers
perform visual actions.

YEP_X_ActSeqPack3: 
The Action Sequence Pack 3 plugin is an extension plugin for Yanfly Engine
Plugins' Battle Engine Core. This extension plugin will not work without the
main plugin.

This extension plugin contains the more basic functions used for customized
action sequences on a visual scale. This plugin focuses on camera control
and screen zooming.

YEP_X_AnimatedSVEnemies: This plugin requires YEP_BattleEngineCore.
Make sure this plugin is located under YEP_BattleEngineCore in the
plugin list.

This extension plugin allows you to animate enemies in a number of ways,
from giving static enemies breathing, floating, and scaled attributes to
utilizing animated sideview actors as potential battlers for your enemies
instead of static graphics to help make your enemies appear more lively!

If you are using YEP_X_ActSeqPack2, and would like the ability to add in
floating enemies, place this plugin under YEP_X_ActSeqPack2 as well.

YEP_X_BattleSysATB: 
The Battle System - Active Turn Battle plugin is an extension plugin for
Yanfly Engine Plugins' Battle Engine Core. This extension plugin will not
work without the main plugin.

To use the ATB system, go to the Battle Engine Core plugin and change the
'Default System' setting in the parameters to 'atb'.

The Active Turn Battle system functions in such where battlers will have a
new gauge in battle functioning as their turn gauge. As time goes by without
anything happening such as actions, menu selection, etc, the gauge fills up.
Once it is full, the battler can commit to an action.

After committing to an action, the battler charges the skill before using it
in battle to either attack an enemy, heal an ally, etc. Upon finishing the
action, the gauge drains to empty and the battler must charge it up again.

This is a battle system where agility plays an important factor in the
progress of battle where higher agility values give battlers more advantage
and lower agility values give battlers less advantage.

YEP_X_BattleSysCTB: The Battle System - Charge Turn Battle plugin is an extension plugin for
Yanfly Engine Plugins' Battle Engine Core. This extension plugin will not
work without the main plugin.

To use the CTB system, go to the Battle Engine Core plugin and change the
'Default System' setting in the parameters to 'ctb'.

The Charge Turn Battle system functions by calculating every battlers' speed
and balancing them relative to one another. When it's a battler's turn, the
battler will either choose an action to perform immediately or charge it for
later depending if the skill requires charging.

This is a battle system where agility plays an important factor in the
progress of battle where higher agility values give battlers more advantage
and lower agility values give battlers less advantage.

YEP_X_BattleSysSTB: This plugin requires YEP_BattleEngineCore. Make sure this plugin is located
under YEP_BattleEngineCore in the plugin list.

To use the STB system, go to the Battle Engine Core plugin and change the
'Default System' setting in the parameters to 'stb'.

The Standard Turn Battle system functions off of the Default Turn Battle
system's structure. Action orders are determined by the battlers' AGI values
and they go from highest to lowest. However, actions are not selected at the
start of the turn. Instead, the turn progresses and the actions are picked
as each battler's turn appears, then proceeds to be executed immediately.

Each battler is only allowed one action per battle turn, meaning a single
battler cannot have twice the number of turns as another battler even if the
battler's AGI value is double that of the other. This is to prevent any
balancing issues that come from tick-based battle systems as they tend to be
far more difficult to balance compared to turn-based battle systems.

Because of the nature of the Standard Turn Battle System, an item or skill's
action speed value found in the database will be disabled as it cannot push
forward a battler's in the turn order.

YEP_X_CoreUpdatesOpt: This plugin requires the following:
- YEP_CoreEngine plugin installed
- Installing this plugin under YEP_CoreEngine
- RPG Maker MV version base code 1.4.0 or above
- Follow the instructions listed in the Help File's "Instructions" section

Does your game project have at least base code (rpg_x.js) 1.4.0 or above?
And has RPG Maker MV updated past that, but you don't feel like updating the
base code manually, probably because you've made some edits to the code
itself? Yet, you still want to take advantage of the changes from the
version ups? This plugin will take care of that for you while keeping your
base code intact, while 'patching' the changes made from higher version ups.

This plugin also adds in the updates and new functions from the versions
leading up to 1.5.2 to ensure that your project has the most up to date
functions even if it is running 1.4.0. This way, you do not have to tamper
with the game project's base code files yourself.

Note: you will still have to download the newest Pixi libraries and to get
things working properly with this plugin. More will be explained in this
plugin's instructions section under the help file.

YEP_X_ExtMovePack1: This plugin requires YEP_MoveRouteCore. Make sure this plugin is located
under YEP_MoveRouteCore in the plugin list.

This plugin adds extra simplified move routes for your events with the main
intention of creating specific behaviors in movement patterns. The patterns
include the option to hug a side of the wall and move along that, moving a
single direction until coming to a stop, relative opacity adjusting, and
index shifting.

YEP_X_ItemUpgradeSlots: This plugin requires YEP_ItemCore.
Make sure this plugin is located under YEP_ItemCore in the plugin list.

This plugin adds Item Upgraders, where you can select the base item and then
apply the appropriate Item Upgraders onto it to boost its parameters.

YEP_X_SkillCooldowns: This plugin requires YEP_SkillCore.
Make sure this plugin is located under YEP_SkillCore in the plugin list.

This plugin allows you to give your skills cooldowns. Cooldowns are a limit
enforced on a skill to prevent them from being used constantly.





















