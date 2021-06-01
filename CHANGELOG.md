# CHANGELOG
**v5.6**<br>
*feature*	: Ability to change mob keywords with `xset kw <mob name>`. When given a mob name it will update the keyword for the currently targeted mob. Without supplying a mob name it will open a series of dialog boxes to rename any mob. https://github.com/AardNaricain/Search-and-Destroy/pull/1<br>
*feature*   : Reorder the list of rooms to look for a mob based on the number of times you have seen it there already. https://github.com/AardCrowley/Search-and-Destroy/pull/3 and https://github.com/AardCrowley/Search-and-Destroy/pull/4<br>
*feature*   : Scan and consider improvements https://github.com/AardCrowley/Search-and-Destroy/pull/5
  * Added a new setting, `xset autocon`, to enable automatically doing a consider when travelling to a room with `nx` or `go`. If your current target is not found it will then perform a scan. Any mobs found in the current room are added to the mobs database.
  * Tag mobs in scan and consider with [GQ] when part of a gquest, [CP] when part of a campaign, and [Q] when part of a quest
  * If autocon is disabled, it will now perform a full scan instead of a quick scan. The new tags should make this more informative.
  * Play a sound when your current target is found in the current room (via scan or consider), a different sound when a non-active target is found in the current room, and a third sound if a target is found nearby according to scan. Toggled with `xset sound` and expects soundpack to be enabled for full functionality.<br>

*feature*   : Quest targets show up in the target window when you're on a quest, and quest status shows up when you've either killed the target or when you can take a quest. https://github.com/AardCrowley/Search-and-Destroy/pull/6<br>
*feature*   : `xcp` with no arguments optionally targets the quest mob. Toggle this behaviour with `xcp quest` https://github.com/AardNaricain/Search-and-Destroy/pull/8<br>
*feature*   : New command `xqt` will target the quest mob https://github.com/AardCrowley/Search-and-Destroy/pull/9<br>
*fix*       : Migrating Pwar's database should be nearly instantaneous. https://github.com/AardNaricain/Search-and-Destroy/pull/1<br>


**v5.5**<br>
*fix*       : Migrating Pwar's database would not work because the SnDdb database was not created yet. Fixed.<br>
*fix*       : Quick kill commands would not accept multiple word commands.<br>
*feature*   : 'xhelp summary' will provide a summary of all commands. For more details, visit each help file.<br>

**v5.4**<br>
*fix*       : The quick kill command was not executing single letter commands. Now fixed.<br>
**v5.3**<br>
*fix*       : Fixed (hopefully) instances where the mob is killed in one hit and not added to mob database.<br>

**v5.2**<br>
*fix*       : Fixed all the previous bugs relating to indexing errors.<br>
*fix*       : Added 'ak' back to the public version and fixed the bug that would split commands erroneously.<br>

**v5.1**<br>
*fix*       : Attempted to fix, failed misrable. See 5.2.<br>

**v5.0**<br>
*feature*   : Added long-awaited mob database!<br>
*feature*   : Added 'snd reload' so you do not have to open Plugins to reinstall.<br>
*change*    : Changed how the help files look. See 'xhelp' for more info.<br>
*Notes*     : Still working on a fix for a couple bugs, but wanted to push this out in the meantime.<br>

**v4.60**<br>
*feature*   : Added changelog per request.<br>
*update*    : Updated the Readme.<br>
*change*    : Changed "Send" to "Execute" on kill command. If there are any problems then blame it on someone else!<br>

**Previous versions**<br>
*update*    : Not going to go through all the updates made. Will update this log going forward.