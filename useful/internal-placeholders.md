---
description: List of Internal Placeholders
---

# 🎯 Internal Placeholders

### BattlePass  & Category GUI:

<table><thead><tr><th width="205.35546875">Placeholder</th><th>Description</th><th>Options</th></tr></thead><tbody><tr><td><code>%pass%</code></td><td>The battlepass name</td><td>add <code>_id</code> for the battlepass ID</td></tr><tr><td><code>%pass_type%</code></td><td>The type of pass the player has (Free/Premium)</td><td></td></tr><tr><td><code>%start_date%</code></td><td>The date the battlepass starts</td><td></td></tr><tr><td><code>%end_date%</code></td><td>The date the battlepass ends</td><td></td></tr><tr><td><code>%tier%</code></td><td>The battlepass tier/level</td><td>add <code>_numeral</code> for numerals</td></tr><tr><td><code>%tier_x%</code></td><td>The battlepass tier +x levels. Eg. <code>%tier_-5%</code> would be current tier, minus 5</td><td>add <code>_numeral</code> for numerals</td></tr><tr><td><code>%claimable_tiers%</code></td><td>The amount of unclaimed tiers.</td><td></td></tr><tr><td><code>%max_tiers%</code></td><td>The max amount of tiers in the pass</td><td></td></tr><tr><td><code>%current_bp_xp%</code></td><td>The current tier XP</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%required_bp_xp%</code></td><td>The XP required for the tier</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%current_task_xp%</code></td><td>The current task XP</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%required_task_xp</code></td><td>The XP required for the task</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%percentage_progress%</code></td><td>The percentage of the tier XP progress</td><td></td></tr></tbody></table>

### BattlePass Tiers GUI

All of the placeholders from BattlePass GUI work here, additionally, you can use the below:

| Placeholder         | Description                      | Options                                           |
| ------------------- | -------------------------------- | ------------------------------------------------- |
| `%free-rewards%`    | The free rewards for the tier    | add `claimed-` prefix for claimed free rewards    |
| `%premium-rewards%` | The premium rewards for the tier | add `claimed-` prefix for claimed premium rewards |

### Quest GUI

|                   |                                              |                                 |
| ----------------- | -------------------------------------------- | ------------------------------- |
| `%category_name%` | Name of the category                         | add `_id` for the category ID   |
| `%pass%`          | Name of the battlepass                       | add `_id` for the battlepass ID |
| `%completed%`     | Number of quests completed in the category   |                                 |
| `%total%`         | Total number of quests in the category       |                                 |
| `%time%`          | Time until the category start/reset/end time |                                 |

### Tasks Lore

| Placeholder          | Description                      | Options                     |
| -------------------- | -------------------------------- | --------------------------- |
| `%task%`             | The name of the task             | add `_id` for the task ID   |
| `%current_task_xp%`  | Player's current XP in the task  | add `_formatted` for commas |
| `%required_task_xp%` | XP required to complete the task | add `_formatted` for commas |

### Other Internal Placeholders

| Placeholder  | Description         |                                          |
| ------------ | ------------------- | ---------------------------------------- |
| `%level%`    | The battlepass tier | Useful for math inside battlepass config |
| `%page%`     | The page number     | Available in Category and Quest GUIs     |
| `%category%` | The category name   | Available for Quest GUI title            |
