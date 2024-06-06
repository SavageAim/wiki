---
description: In-depth explanation about the Loot Manager's "Solver" feature.
---

# Loot Solver

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>Loot Solver with the Per Fight Loot Manager</p></figcaption></figure>

{% hint style="warning" %}
Please note this is a Beta feature that makes a few assumptions in order to work. Read this page for full information.
{% endhint %}

## How it Works

The Solver will parse your Team's required items and build a plan to hand out loot in a way that is as fair as possible while optimizing for minimum required weeks to be done with a fight.

As it is a Beta feature, it makes some assumptions, which will be listed below!

For any fight, if there are required kills remaining, you can see the forecasted Loot Distribution using the "See Distribution" button. This will display a pop-up that looks something like this;

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Any square marked "Greed" will be free for Greed rolls.

Clicking the "Auto Assign" button (only available if you're using the [per-fight-loot-manager.md](per-fight-loot-manager.md "mention")), you can have the Loot Manager automatically switch the fight to the selected one, and then populate the slots automatically, ready for you to hit Save.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The Loot Solver does not forecast for Tome Weapon Tokens, or Tome Weapon Augments. These should be handled manually, for whoever has the tomes available to buy them or however else you wish to hand them out!
{% endhint %}

### Algorithm

* For each floor, determine how many Team Members need each possible item (excluding Tome Weapon Tokens and Upgrades)
* Generate a map between the number of items needed, and the list of Members who need that many items.
  * These lists will be sorted based on the Team's Solver Sort;
    * The default order is Melee > Phys Ranged > Caster > Tank > Healer, with Jobs that were released first coming first in ties for roles.
    * This order can be overridden in the [team-settings.md](team-settings.md "mention") page.
  * This map is then used to be our priority system
* Simulate kills, handing out items in descending order of priority, and handling purchases with tokens when the requisite amount is obtained, until everyone has everything they need from the fight.
  * When a Member is given an item, they are added to the end of the list for the new number of items they require
  * This is so the Solver is as fair as possible, as it discourages handing the same Member items back-to-back unless they are the only one who needs something.

### Split Clears

{% hint style="info" %}
Split Clears - The act of using alts to perform two clears in a week of one fight, to double the speed at which everyone in the Team gets geared.
{% endhint %}

This section is here to just touch on the subject. Since the number of clears for tracking tokens is based on the unique dates that History items have, I think split clearing will not fully work with the system.&#x20;

If you are a split clear group using the Solver, and it has issues, then feel free to let us know on the Discord!

## Assumptions

### Spending Tokens

Whenever you clear a fight, you receive a token. For a number of these tokens, you can buy loot to speed up gearing.

{% hint style="warning" %}
Where possible, the algorithm assumes you will buy Upgrade Tokens for Tome gear, and then will assume you buy items in the following order of possible items;\
\
Head > Body > Hands > Legs > Feet > Earrings > Necklace > Bracelet > Ring
{% endhint %}

### BIS Lists Are Up To Date

The Solver algorithm checks through the History to see what Loot was assigned, and it also checks each Member's BIS Lists to see what extra items they have BIS that weren't tracked.

This allows for Members joining halfway through a tier, pre-geared, to not break the system, but it also means that on weeks when Tokens are spendable, it handles the acquisition of Gear outside of the Loot History.

That being said, whenever Members are given Augment tokens / can buy things, the Solver expects that each Member will update their own BIS on their own.
