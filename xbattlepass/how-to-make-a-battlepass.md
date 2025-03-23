# How to make a BattlePass

The `battlepass.yml` is the key to your BattlePass. This is where you define how much XP is needed per-tier, how many tiers are in the BattlePass, and what rewards the player receives.

## Default configs
The default configs can be found here.

> [!example]
> 
> ```yaml
> battlepass:
>   xp-formula: 1.5 * %level% + 5 # The formula to calculate the XP needed to reach the next tier
>   max-tier: 100 # The maximum tier of the battle pass
>   command: 'battlepass' # The command to open the battle pass GUI
>   premium-permission: exanthiax.pass.premium # The permission to access the premium tiers
>   battlepass-start: 2025-01-01 00:00 # The date the battle pass starts
> 
> tiers:
>   - tier: 1
>     rewards: # The ID of the reward
>       - id: diamond_block
>         tier: free # The tier the reward is in (free/premium/both)
>       - id: money_1000
>         tier: premium
>   - tier: 5
>     rewards: # The ID of the reward
>       - id: money_5000
>         tier: free
>   - tier: 15
>     rewards: # The ID of the reward
>       - id: skeleton_spawner
>         tier: premium
> ```