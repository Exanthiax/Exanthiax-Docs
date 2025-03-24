# Configuring a Category

## Default config

The default config can be found here.

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
