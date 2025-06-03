# PlaceholderAPI



{% tabs %}
{% tab title="Internal Placeholders" %}
<table><thead><tr><th width="205.35546875">Placeholder</th><th>Description</th><th>Options</th></tr></thead><tbody><tr><td><code>%level%</code></td><td>The battlepass tier/level.</td><td>add <code>_numeral</code> for numerals</td></tr><tr><td><code>%next_tier%</code></td><td>The next battlepass tier/level.</td><td>add <code>_numeral</code> for numerals</td></tr><tr><td><code>%claimable_tiers%</code></td><td>The amount of unclaimed tiers.</td><td></td></tr><tr><td><code>%pass%</code></td><td>The battlepass name.</td><td></td></tr><tr><td><code>%current_bp_xp%</code></td><td>The current tier XP.</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%required_bp_xp%</code></td><td>The XP required for the tier.</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%current_task_xp%</code></td><td>The current task XP.</td><td>add <code>_formatted</code> for commas</td></tr><tr><td><code>%required_task_xp</code></td><td>The XP required for the task.</td><td>add <code>_formatted</code> for commas</td></tr></tbody></table>


{% endtab %}

{% tab title="PlaceholderAPI" %}
| Placeholder                               | Description                            | Options                     |
| ----------------------------------------- | -------------------------------------- | --------------------------- |
| `%xbattlepass_category_<id>_start_date%`  | The start date of the quest category.  |                             |
| `%xbattlepass_category_<id>_end_date%`    | The end date of the quest category.    |                             |
| `%xbattlepass_category_<id>_start_timer%` | the time until the category starts.    |                             |
| `%xbattlepass_category_<id>_end_timer%`   | The time until the category ends.      |                             |
| `%xbattlepass_category_<id>_reset_timer%` | The time until the category resets.    |                             |
| `%xbattlepass_claimable_<battlepass>%`    | The amount of claimable tiers/rewards. |                             |
| `%xbattlepass_tier_<battlepass>%`         | The player's current Battlepass tier.  | add `_numeral` for numerals |
| `%xbattlepass_xp_<battlepass>%`           | The player's current tier xp.          | add `_formatted` for commas |
| `%xbattlepass_xp_required_<battlepass>%`  | The amount of xp needed for the tier.  | add `_formatted` for commas |
{% endtab %}
{% endtabs %}
