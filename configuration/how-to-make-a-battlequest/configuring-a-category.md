# Configuring a Category

## Default config

The default config can be found here.

## How to add categories

Each quest is its own config file, placed in the `/categories/` folder, and you can add or remove them as you please. There's an example config called `_example.yml` to help you out!

The ID of the Category is the file name. ID's must be lowercase letters, numbers, and underscores only.

Categories allow both Free and Premium quests

## Example Category Config

```yaml
name: "&8»&e Daily Challenges"
item: nether_star 1
lore:
  - "&a%completed%/%total% Complete"

battlepass: battlepass
priority: 0
start-date: 2025-03-23 00:00
duration: 100000
reset-time: 1440

quests:
  - id: free_daily_quest_1
  - id: free_daily_quest_2
  - id: free_daily_quest_3
```

### Understanding the Sections

#### The Display Section:

```yaml
# The display name, display item, and lore of the category. This shows in the Categories GUI.
name: "&8»&e Daily Challenges"
item: nether_star 1
lore:
  - "&a%completed%/%total% Complete"
  - "%xbattlepass_category_daily_duration%"
```
#### The Config Section:

```yaml
# The ID of the battlepass this category is assigned to.
battlepass: battlepass
# The priority of the category in the GUI. Categories are sorted by priority, 0 is the highest priority, and will show first.
priority: 0
# The date the category starts.
# Format: YYYY-MM-DD HH:MM
start-date: 2025-03-23 00:00
# The duration of the category in minutes, set to -1 for no end.
# This allows you to end/lock categories after a time frame.
duration: 100000
# The amount of minutes between resets. 
# Set to 1440 for daily resets, set to -1 for no reset.
reset-time: 1440
```

#### The Quests Section

```yaml
# The list of Quest ID(s) to be completed.
# The order of this list is what determines the order within the Category GUI.
quests:
  - id: free_daily_quest_1
  - id: free_daily_quest_2
  - id: free_daily_quest_3
```

#### Internal Placeholders

| Placeholder   | Value                                           |
| ------------- | ----------------------------------------------- |
| `%completed%` | The amount of completed quests in the category. |
| `%total%`     | The total amount of quests in the category.     |
