---
description: >-
  An in-depth look at the loot management and tracking system built into Savage
  Aim
---

# Loot Manager

![](<../.gitbook/assets/image (2).png>)

The Loot Manager is a semi-automated system of determining who needs what raid loot, and also a tracker of historical data for a Team throughout each Tier of their progress.

This page will go through each of the sections to the Loot Manager and explain how they work.

## What Item Dropped

![](<../.gitbook/assets/image (21).png>)

In the box at the top of the page is a single dropdown input. This input contains the names of all of the item slots that can have gear drop for them.

Picking an item from this list will trigger the Need and Greed sections to activate.

## Need

![](<../.gitbook/assets/image (1).png>)

![](<../.gitbook/assets/image (23).png>)

The Need box starts like the first image. When an item is selected in the What Item Dropped selection, it gets populated like the second image.

The Need box is populated as follows;

* Every Character in the team has their **linked BIS List** checked
* If a Character's BIS List needs the raid drop for the chosen slot, and does not currently have it, they are displayed here.

To get the second image, I selected "Body" from the Item drop. I can see that I appear in the list, meaning my main job needs the Body from raid.

### List Item Breakdown

Each item in the list will look like as displayed in the second image. A full description of what is displayed is as follows.

#### Character Name

As in other pages, this will display the name and home world of the Character.

#### Item Level Tag

Similarly to [#item-level-tag](team-details.md#item-level-tag "mention") on the Details page, a depiction of item level is displayed on the right side. However, instead of displaying the Character's current item level of their BIS List, this tag instead describes the current item level of **the currently equipped gear in the slot**.&#x20;

#### Job Icon

Also displays the Job icon here for consistency with the [#heading](team-details.md#heading "mention") of cards in the Details page.

#### Give Item

If the Team Leader is looking at the Loot Manager, they will also get this button.

Clicking this button will do two things.

1. Creates an entry in the Team's Loot History to keep track of who gets what.
2. Updates the Character's BIS List to set their current gear to be the raid item.

To avoid #2, you can also [#track-loot-manually](loot-manager.md#track-loot-manually "mention").

#### Hover / Tap

Also like the Team Details page, hovering or tapping the box displays the Current Gear tooltip.

## Greed

![](<../.gitbook/assets/image (3).png>)

![](<../.gitbook/assets/image (12).png>)

Similarly to the Need section above, the Greed section starts like the first image. When an item is selected, it becomes like the second picture.&#x20;

However, Greed is populated in a different way to Need.

* The system checks all of a Character's BIS Lists, **excluding the one linked to the Team**.
* If any of the Character's other BIS Lists need the raid gear for the chosen slot, they get displayed.

Similar to Need, there will be one dark box per character. However, as you can see above, there can be multiple entries in the box, depending on how many BIS Lists the Character has that needs the chosen slot.

Everything else works the same as described in Need. The "Give Item" buttons will update the BIS List associated with whichever row you press the button for.

## Loot History

The Loot History box starts minimised, but clicking / tapping on it will expand it to display something like this.

![](<../.gitbook/assets/image (20).png>)

Each row in the table indicates the date the item was obtained, the Character that received it, the Item that was received, and whether the item was Needed or Greeded.

{% hint style="info" %}
When you change to a new Tier, the History table will be empty. This is because Loot History is tracked per Tier. To view your old Loot History, the Team Leader can change the Team's Tier back temporarily.
{% endhint %}

Using the "Give Item" button as the Team Leader will automatically fill in the Need/Greed text as appropriate. This button will also set the date obtained to the day you clicked the button, since the system assumes you use this button right as you get the items.

{% hint style="info" %}
This is how my static handles things. Maybe the Need/Greed differentiation is unnecessary for you but it doesn't affect anything whether a roll was Need or Greed.
{% endhint %}

However, there are some items that don't give raid gear, or aren't gear at all, or you forgot to track an item you obtained last week. If you want to track these, or you don't want to to use the "Give Item" buttons at all, there is another option.

### Track Loot Manually

At the bottom of the above image is a row containing inputs. Like the "Give Item" buttons, this row is only available to the Team Leader.

Using this extra row, it is possible to add arbitrary History records.

You can add items from the past, to any Character, and the Item dropdown contains more items than the "What Item Dropped" dropdown above. The extra items are;

* Tome Weapon Token
* Tome Accessory Augment
* Tome Armour Augment
* Tome Weapon Augment
* Mount

{% hint style="info" %}
Taking the Augment items and putting them into the Need/Greed sections above is something on our minds!
{% endhint %}

Then you can click either Need or Greed to submit the request. If all is successful the item should appear in the list, otherwise red error text will be displayed next to whichever inputs are reporting errors.
