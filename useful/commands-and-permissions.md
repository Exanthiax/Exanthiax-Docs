---
description: List of Commands and Permissions
---

# Commands & Permissions

{% tabs %}
{% tab title="Permissions" %}
### Premium Battlepass

To set the permission required for the Premium Battlepass, edit this in your battlepass configs.

### XP multiplier permission

Permission: `xbattlepass.xpmultiplier.<%increase>`

General Usage: `xbattlepass.xpmultiplier.200` would give 200% more battlepass XP (3x) to anyone with the permission. The backend math is `1 + (<%increase> / 100)` so

Permission: `xbattlepass.xpmultiplier.50percent Permission:` xbattlepass.xpmultiplier.double`Permission:`xbattlepass.xpmultiplier.triple`Permission:`xbattlepass.xpmultiplier.quadruple\`

General Usage: `xbattlepass.xpmultiplier.50percent` would give 50% more skill XP (1.5x)
{% endtab %}

{% tab title="Commands" %}
## `Open Battlepass GUI (eg: /Battlepass)`

This is the command to open the Battlepass GUI\
Usage: `/battlepass, /eventpass, etc.`\
Permission: \`xbattlepass.command.

Eg. A battlepass with the command `/eventpass` would be `xbattlepass.command.eventpass`

## `/xbattlepass give`

The command to give battlepass XP\
Usage: `/xbattlepass give <player/all> <battlepass_id> <tier/xp> <amount>`\
Permission: `xbattlepass.command.give`

## `/xbattlepass reload`

The command to reload the plugin and configs\
Usage: `/xbattlepass reload`\
Permission: `xbattlepass.command.reload`

## `/xbattlepass reset`

The command to reset battlepass XP\
Usage: `/xbattlepass reset <player/all> <battlepass_id>`\
Permission: `xbattlepass.command.reset`

## `/xbattlepass tier`

The command to open the Battlepass tiers GUI\
Usage: `/xbattlepass tier <battlepass_id>`\
Permission: `xbattlepass.command.tier`

## `/xbattlepass quests`

The command to open the Battlepass quests GUI\
Usage: `/battlepass quests <battlepass_id>`\
Permission: `xbattlepass.command.quests`
{% endtab %}
{% endtabs %}

###

### Premium Battlepass

To set the permission required for the Premium Battlepass, edit this in your battlepass configs.

### XP multiplier permission

Permission: `xbattlepass.xpmultiplier.<%increase>`

General Usage: `xbattlepass.xpmultiplier.200` would give 200% more battlepass XP (3x) to anyone with the permission. The backend math is `1 + (<%increase> / 100)` so

Permission: `xbattlepass.xpmultiplier.50percent Permission:` xbattlepass.xpmultiplier.double`Permission:`xbattlepass.xpmultiplier.triple`Permission:`xbattlepass.xpmultiplier.quadruple\`

General Usage: `xbattlepass.xpmultiplier.50percent` would give 50% more skill XP (1.5x)

## `Open Battlepass GUI (eg: /Battlepass)`

This is the command to open the Battlepass GUI\
Usage: `/battlepass, /eventpass, etc.`\
Permission: \`xbattlepass.command.

Eg. A battlepass with the command `/eventpass` would be `xbattlepass.command.eventpass`

## `/xbattlepass give`

The command to give battlepass XP\
Usage: `/xbattlepass give <player/all> <battlepass_id> <tier/xp> <amount>`\
Permission: `xbattlepass.command.give`

## `/xbattlepass reload`

The command to reload the plugin and configs\
Usage: `/xbattlepass reload`\
Permission: `xbattlepass.command.reload`

## `/xbattlepass reset`

The command to reset battlepass XP\
Usage: `/xbattlepass reset <player/all> <battlepass_id>`\
Permission: `xbattlepass.command.reset`

## `/xbattlepass tier`

The command to open the Battlepass tiers GUI\
Usage: `/xbattlepass tier <battlepass_id>`\
Permission: `xbattlepass.command.tier`

## `/xbattlepass quests`

The command to open the Battlepass quests GUI\
Usage: `/battlepass quests <battlepass_id>`\
Permission: `xbattlepass.command.quests`
