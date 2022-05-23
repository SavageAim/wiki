---
description: >-
  An in-depth look at the loot management and tracking system built into Savage
  Aim
---

# Loot Manager

![](<../.gitbook/assets/image (3) (1) (1) (1).png>)

The Loot Manager is a semi-automated system of determining who needs what raid loot, and also a tracker of historical data for a Team throughout each Tier of their progress.

This page will go through each of the sections to the Loot Manager and explain how they work.

## What Item Dropped

![](<../.gitbook/assets/image (28) (1).png>)

In the box at the top of the page is a single dropdown input. This input contains the names of all of the item slots that can have gear / items drop for them.

Picking an item from this list will trigger the Need and Greed sections to activate.

## Need

![](<../.gitbook/assets/image (1) (1) (1).png>)

![](<../.gitbook/assets/image (16) (1).png>)

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

To avoid #2, you can also [#track-loot-manually](loot-tracker.md#track-loot-manually "mention").

{% hint style="warning" %}
Please note that for rings, the request will update whichever slot whose BIS is set to the raid gear. Please ensure that this doesn't mess with your current gear, i.e. overriding a tome ring instead of a crafted ring.

If your item level on Savage Aim doesn't match FFXIV, and you've recently received ring loot, then this could be why.
{% endhint %}

#### Hover / Tap

Also like the Team Details page, hovering or tapping the box displays the Current Gear tooltip.

#### Numbered Badge

In the above picture, there is a circular badge with a 0 in it. This indicates that the Character has received 0 pieces of Need loot so far this Tier. This makes round-robin style obtaining of loot (the style my own static uses) easier to calculate!&#x20;

Need entries will have light blue badges, and greed entries will have purple badges, to match the colours used for need/greed elsewhere on the page.

## Greed

![](<../.gitbook/assets/image (4) (1) (1).png>)

![](<../.gitbook/assets/image (15).png>)

Similarly to the Need section above, the Greed section starts like the first image. When an item is selected, it becomes like the second picture.&#x20;

However, Greed is populated in a different way to Need.

* The system checks all of a Character's BIS Lists, **excluding the one linked to the Team**.
* If any of the Character's other BIS Lists need the raid gear for the chosen slot, they get displayed.
* However, if a Character has no lists that match the item, they will also be displayed for Quality of Life purposes, instead of requiring people to use the manual update.

Similar to Need, there will be one dark box per Character, with a purple badge indicating how much Greed loot has been obtained by them.&#x20;

However, due to Characters being able to have multiple BIS Lists that aren't associated with the Team, there is a second layer to the system for Greed lists. When giving loot to a Character with a Greed BIS List, the "Select BIS" button will take you to a popup that looks like this.

![](<../.gitbook/assets/image (20).png>)

Clicking one of these lists will update them, just like the Need section. However, the Greed side also contains entries for Characters with no extra BIS Lists on the website. This just makes it easier to add History entries for them in case they also get Greed loot.

## Tome Augmentation Items

In addition to tracking who needs what raid gear drops, the Loot Manager can also track how many augmentation tokens Characters need for both Tome Armour and Accessories. Due to the slight difference in what this information needs to display, the entries for Tome Augmentation items look slightly different that what is outlined in the above section.

![](<../.gitbook/assets/image (23) (1) (1).png>)![](<../.gitbook/assets/image (10) (1).png>)

### Requires

The most important difference between Tome and Raid items in the Loot Manager is that Tome items are augmentation tokens, and normally Characters will need multiple to complete their BIS.

Instead of displaying a currently equipped item name in the tooltip, or the item level currently equipped in the tag (on desktop), when a Tome Augment item is selected both will instead indicate how many of the item are needed for each BIS List.

On Mobile view, the requires number is instead displayed as a dark blue badge to the left of each entry, and is still available in the tooltip when the entry is tapped on.

### Give Item

Due to the nature of the items in question, when passing out loot via the Loot Manager for Tome Augment tokens, we cannot automatically update the BIS in question. We cannot set a way to pick slots via the UI, nor do we want to tie Characters into knowing what piece of Gear they want to upgrade beforehand.

Due to these points, it has been decided to prevent Tome Augment tokens from automatically update anyone's BIS Lists. Instead, they will just be tracked like the other items, and will be entered into the Loot History table just the same as handing out raid items would be.

## Loot History

The Loot History box starts minimised, but clicking / tapping on it will expand it to display something like this.

![](<../.gitbook/assets/image (16).png>)![](<../.gitbook/assets/image (7).png>)

Each row in the table, or block in the mobile version to the right, indicates the date the item was obtained, the Character that received it, the Item that was received, and whether the item was obtained through Need or Greed.

{% hint style="info" %}
When you change to a new Tier, the History will be empty. This is because Loot History is tracked per Tier. To view your old Loot History, the Team Leader can change the Team's Tier back temporarily.
{% endhint %}

Using the "Give Item" button as the Team Leader will automatically fill in the Need/Greed text as appropriate. This button will also set the date obtained to the day you clicked the button, since the system assumes you use this button right as you get the items.

{% hint style="info" %}
This is how my static handles things. Maybe the Need/Greed differentiation is unnecessary for you but it doesn't affect anything whether a roll was Need or Greed.
{% endhint %}

However, there are some items that don't give raid gear, or aren't gear at all, or you forgot to track an item you obtained last week. If you want to track these, or you don't want to to use the "Give Item" buttons at all, there is another option.

### Track Loot Manually

At the bottom of the above images is a section containing inputs. Like the "Give Item" buttons, this row is only available to the Team Leader.

Using this extra form, it is possible to add arbitrary History records.

You can add items from the past, to any Character, and the Item dropdown contains more items than the "What Item Dropped" dropdown above. The extra items are;

* Tome Weapon Token
* Tome Weapon Augment
* Mount

Then you can click either Need or Greed to submit the request. If all is successful the item should appear in the list, otherwise red error text will be displayed next to whichever inputs are reporting errors.

### Deletion

![](<../.gitbook/assets/image (28) (1) (1).png>)

If necessary, the Team Leader may delete Loot History records. This feature has been provided in case an error is made when using the Loot Manager.

{% hint style="danger" %}
Please note that deleting an entry that also updated a Character's BIS List will not revert the changes to the BIS List. Please be careful using the Loot Manager automated functions.
{% endhint %}

In the above images, Desktop users (image on the left) may delete multiple entries at once, using the checkboxes and Delete button in the bottom table row.

Mobile users (image on the right) however must delete entries one at a time using the individual Delete buttons associated with each entry.

Both platforms will receive a confirmation popup that must be accepted before any deletion will occur.
