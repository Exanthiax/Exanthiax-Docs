# Configuring a Quest

## Default configs

The default configs can be found here.

## How to add quests

Each quest is its own config file, placed in the `/quests/` folder, and you can add or remove them as you please. There's an example config called `_example.yml` to help you out!

The ID of the Quest is the file name. This is what you use in your Categories.\
ID's must be lowercase letters, numbers, and underscores only.

## Example Quest Config

```yaml
display:
  item: player_head texture:"eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvNGU4ZjNlYTQ2NzM1YWQwYzEwNmM1NDljY2I2Y2Q0ODljOTdhNDFlNzNkMDkyNDk3ZWU0MjRiZWNkOWRmZDI5YyJ9fX0="
  display-name: Chickens
  description:
    - "Kill animals to earn points"

battlepass-points: 100
battlepass-tier: premium 

tasks:
  - id: chickens
    xp: 100

task-amount: 1
```

### Understanding the Sections

#### The Display Section:

```yaml
display:
  # The item to show in the GUI. Read here for more: 
  # https://plugins.auxilor.io/all-plugins/the-item-lookup-system.
  item: player_head texture:"eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvNGU4ZjNlYTQ2NzM1YWQwYzEwNmM1NDljY2I2Y2Q0ODljOTdhNDFlNzNkMDkyNDk3ZWU0MjRiZWNkOWRmZDI5YyJ9fX0="
  # The display name and description of the Quest.
  display-name: Chickens
  description:
    - "Kill animals to earn points"
```

[Item Lookup System](https://plugins.auxilor.io/all-plugins/the-item-lookup-system).

#### The Config Section

```yaml
# The amount of BattlePass XP to be awarded
battlepass-points: 100
# If the Quest is for Premium, or Free BattlePasses.
# If you choose "Free", Premium users can still progress.
battlepass-tier: premium 
```

#### The Tasks Section

```yaml
tasks:
    # Here goes the ID(s) of the Task(s) to be completed.
  - id: chickens
    # The task XP required. 
    xp: 100

# The amount of Tasks from the list required to be completed.
# Used if you want players to complete 2/3 options.
task-amount: 1
```
