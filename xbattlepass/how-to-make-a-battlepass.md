# How to make a BattlePass

The `battlepass.yml` is the key to your BattlePass. This is where you define how much XP is needed per-tier, how many tiers are in the BattlePass, and what rewards the player receives.

## Default configs
The default configs can be found here

## Example BattlePass Config

```yaml
battlepass:
  xp-formula: 1.5 * %level% + 5
  max-tier: 100
  command: 'battlepass'
  battlepass-start: 2025-01-01 00:00

tiers:
  - tier: 1
    rewards: # The ID of the reward
      - id: diamond_block
        tier: free # The tier the reward is in (free/premium/both)
      - id: money_1000
        tier: premium
  - tier: 5
    rewards: # The ID of the reward
      - id: money_5000
        tier: free
  - tier: 15
    rewards: # The ID of the reward
      - id: skeleton_spawner
        tier: premium
```

## Understanding the Sections

#### The BattlePass Configuration
```yml
battlepass:
  # The formula to calculate the XP needed to reach the next tier.
  xp-formula: 1.5 * %level% + 5
  
  # The maximum tier of the BattlePass.
  max-tier: 100
  
  # The command used to open the BattlePass GUI.
  command: 'battlepass'
  
  # The date and time the BattlePass starts. Format: YYYY-MM-DD HH:MM
  # This uses the server time, you cannot specify a timezone.
  battlepass-start: 2025-01-01 00:00
```

#### The Reward Tiers
```yaml
tiers:
	# The tier number for the reward(s).
	# Don't include the tier if you don't want a reward.
  - tier: 1
    rewards:
	    # The ID of the reward, see more here:
      - id: diamond_block
	    # The tier the reward is in.
	    # "Premium" means only Premium players, "Free" allows anyone to claim
        tier: free
        # List all the rewards in the same format.
      - id: money_1000
        tier: premium
```

