# Commands & Permissions

### Premium Battlepass
To set the permission required for the Premium Battlepass, edit this in config.yml

### XP multiplier permission

Permission: `xbattlepass.xpmultiplier.<%increase>`

General Usage: `xbattlepass.xpmultiplier.200` would give 200% more battlepass XP (3x) to anyone with the permission. The backend math is `1 + (<%increase> / 100)` so 

Permission: `xbattlepass.xpmultiplier.50percent
Permission: `xbattlepass.xpmultiplier.double`
Permission: `xbattlepass.xpmultiplier.triple`
Permission: `xbattlepass.xpmultiplier.quadruple`

General Usage: `xbattlepass.xpmultiplier.50percent` would give 50% more skill XP (1.5x)

## `/battlepass`

This is the command to open the main Battlepass GUI
Usage: `/battlepass`
Permission: `xbattlepass.command.xbattlepass`

## `/battlepass give`

The command to give battlepass XP
Usage: `/battlepass give <player> <xp-amount>`
Permission: `xbattlepass.command.give`

## `/battlepass reload`

The command to reload the plugin and configs
Usage: `/battlepass reload`
Permission: `xbattlepass.command.reload`

## `/battlepass reset`

The command to give battlepass XP
Usage: `/battlepass reset <player>`
Permission: `xbattlepass.command.reset`

## `/battlepass tier`

The command to open the Battlepass tiers GUI
Usage: `/battlepass tier`
Permission: `xbattlepass.command.tier`

## `/battlepass quests`

The command to open the Battlepass quests GUI
Usage: `/battlepass tier`
Permission: `xbattlepass.command.quests`
