# How to make a BattleQuest

BattleQuests are how players gain BattlePass XP.
They could be something simple, like "Mine 25 Iron Ores", or they can be more complex, like "Kill 32 Zombies, whilst below Y=0, wearing Diamond Leggings and holding a carrot in the off-hand", the choice is yours.

BattleQuests are formed of three components: the task, the quest, and the category.

We will start with Tasks.
## Default configs
The default configs can be found here.

## How to add tasks
Each task is its own config file, placed in the `/tasks/` folder, and you can add or remove them as you please. There's an example config called `_example.yml` to help you out!

The ID of the Task is the file name. This is what you use in your Quests.
ID's must be lowercase letters, numbers, and underscores only.

## Example Task Config

```yaml
display:
  display-name: Chickens
  lore:
    - "&7Kill chickens"
    - "&7%current%/%required%"

xp-gain-methods:
  - trigger: kill
    value: 1
    filters:
      entities:
        - chicken
```

### Understanding the Sections

#### The Display Section
```yaml
display:
  # The display name and lore of the task, this shows in the Quest.
  display-name: Chickens
  lore:
    - "&7Kill chickens"
    - "&7%current%/%required%"
```
#### Internal Placeholders

| Placeholder  | Value                 |
| ------------ | --------------------- |
| `%current%`  | The current task xp.  |
| `%required%` | The required task xp. |
#### The XP Gain Methods
```yaml
# An XP gain method takes a trigger, a multiplier, conditions, args and filters.
# The 'multiplier' takes the value produced by the trigger and multiplies it
# Alternatively, you can use 'value' to count a specific number and not a multiplier
xp-gain-methods:
  - trigger: kill
    value: 1 # You can also use "multiplier" here.
    filters: # Optional
      entities:
        - chicken
```

Read [here](https://plugins.auxilor.io/effects/all-triggers) for the triggers.

## How to add quests
Each quest is its own config file, placed in the `/quests/` folder, and you can add or remove them as you please. There's an example config called `_example.yml` to help you out!

The ID of the Quest is the file name. This is what you use in your Categories.
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

## How to add categories
Categories are defined in `categories.yml`. This is where you can group quests, such as Daily Quests, Weekly Quests, etc. You simply list the different categories and their attributes.

Categories allow both Free and Premium quests together.
## Example Category Config

```yaml
categories:
  - id: week_1 # The category ID, must be unique
    name: "Week 1 Challenges" # The name of the category
    item: emerald unbreaking:1 hide_enchants
    lore:
      - "&7Week 1 Challenges"
      - "&a%completed%/%total% Complete"
	# The date the category starts.
	# Format: YYYY-MM-DD HH:MM
    start-date: 2025-03-23 00:00
	# The duration of the category in minutes, set to -1 for no end.
	# This allows you to end/lock categories after a time frame.
    duration: 10080
    # The amount of minutes between resets. 
    # Set to 1440 for daily resets, set to -1 for no reset.
    reset-time: 1440
    quests: # The quest ID(s) in the category.
      - id: daily_quest_1
```