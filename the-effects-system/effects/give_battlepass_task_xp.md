# give\_battlepass\_task\_xp

**Triggered Effect**

Gives experience points for a task in a quest, excluding multipliers.

## Example Config

```yaml
- id: give_battlepass_task_xp
  args:
    amount: 100 # The amount of xp to give
    task: chickens # The task ID
    quest: daily_quest_1 # The quest ID
  ...other config (eg triggers, filters, mutators, etc)
```
