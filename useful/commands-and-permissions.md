---
description: List of Commands and Permissions
---

# 💼 Commands & Permissions

| Command                                                                                                                                                                                                                         | Description                                                     | Permission                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- | ---------------------------------- |
| `/<battlepass_id>`                                                                                                                                                                                                              | Open the battlepass GUI                                         | `xbattlepass.command.<pass_id>`    |
| `/xbattlepass reload`                                                                                                                                                                                                           | Reloads the plugin                                              | `xbattlepass.command.reload`       |
| `/xbattlepass quests <pass_id>`                                                                                                                                                                                                 | Opens the Quests GUI                                            | `xbattlepass.command.quests`       |
| `/xbattlepass tier <pass_id>`                                                                                                                                                                                                   | Opens the Tiers GUI                                             | `xbattlepass.command.tier`         |
| `/xbattlepass setpremium <player> <pass_id> <true/false> [silent]`                                                                                                                                                              | Set the player's premium pass                                   | `xbattlepass.command.setpremium`   |
| `/xbattlepass complete_task <player/all> <pass_id> <category_id> <quest_id> <task_id>`                                                                                                                                          | Complete the player's battlepass task                           | `xbattlepass.command.completetask` |
| <p><code>/xbattlepass reset battlepass &#x3C;player/all> &#x3C;pass_id></code> <br><code>/xbattlepass reset task &#x3C;player/all> &#x3C;pass_id> &#x3C;category_id> &#x3C;quest_id> &#x3C;task_id></code></p>                  | Reset the player's battlepass or task experience                | `xbattlepass.command.reset`        |
| <p><code>/xbattlepass give &#x3C;player/all> &#x3C;pass_id> &#x3C;tier/xp> &#x3C;amount></code><br><code>/xbattlepass give &#x3C;player/all> task_xp &#x3C;category_id> &#x3C;quest_id> &#x3C;task_id> &#x3C;amount></code></p> | Give the player battlepass tiers, experience or task experience | `xbattlepass.command.give`         |

### Additional Permissions

#### Premium Battlepass

To set the permission required for the Premium Battlepass, edit this in your battlepass configs.

#### XP multiplier permission

Permission: `xbattlepass.xpmultiplier.<%increase>`

General Usage: `xbattlepass.xpmultiplier.200` would give 200% more battlepass XP (3x) to anyone with the permission. The backend math is `1 + (<%increase> / 100)`&#x20;

Permission: `xbattlepass.xpmultiplier.50percent`\
\
&#x20;\
Permission: `xbattlepass.xpmultiplier.double`\
\
&#x20;\
Permission: `xbattlepass.xpmultiplier.triple`\
Permission: `xbattlepass.xpmultiplier.quadruple`

General Usage: `xbattlepass.xpmultiplier.50percent` would give 50% more skill XP (1.5x)
