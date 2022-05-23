---
description: All about the management of BIS Lists for Characters
---

# BIS Lists

## Tracking Gear

Once you have your Characters imported and set up, we can begin to track the Gear they have versus the Gear they need. To do so, we can create a new BIS List.&#x20;

After importing and verifying a Character, we should be on a page like this;

![](<../.gitbook/assets/image (8) (1) (1).png>)

To add a new BIS List, click the purple "Add New" button to the right of the BIS Lists box.

## Make a New List

You should have ended up on a page that looks something like this;

![](<../.gitbook/assets/image (19).png>)

The form in its current state is quite large, and split into 5 sections; Details, BIS Gear, and Current Gear, which are the details required and maintained, and then a Filters section, which allows for filtering the gear in the dropdowns by a range of item levels. Lastly there is the Actions section which contains various buttons for interacting with the List.

On mobile, the form is split into tabs, and should look something like the below picture when you first load in. The tabs on mobile correspond with the sections above, but keep the mobile UI easier to use!

![](<../.gitbook/assets/image (14).png>)

The Actions section will be displayed below each tab for ease of use.

### Details

![](<../.gitbook/assets/image (3).png>)

In the Details section, you can pick the Job associated with the list, and optionally add a URL and a name.&#x20;

#### Name

An optional name for the BIS List. This will be used in places to potentially differentiate between different BIS Lists for the same job.

Names are used in the [character-details.md](character-details.md "mention") page, as well as the [#bis-list](../teams/create-a-team.md#bis-list "mention") part of the Join Team, Create Team, or Edit Team Membership pages.

#### Job

The Job for which the BIS List is for. Used to display Job icons in various places and also to determine whether Offhand should be tracked separately for Paladins.

#### Extra URL

A URL to any site you want. A link will be displayed under BIS List cards to this website, and is handy to have for easy access to sites like Etro where materia information is stored alongside gear.

{% hint style="info" %}
If you insert an Etro Gearset URL, you will be able to import the BIS Gear straight into Savage Aim as well! See [#import](bis-lists.md#import "mention") for more details.
{% endhint %}

### BIS Gear

![](<../.gitbook/assets/image (17) (1) (1).png>)

This section of dropdowns allows you to pick the Best in Slot gear for the List. The options in the dropdowns are the various types of Gear you can acquire, filtered for what can be equipped in that slot.

{% hint style="info" %}
For any job other than Paladin, the "Off Hand" option will not be available to choose. This is because only Paladin currently has the option to have different types of item in the main and off hand slots.
{% endhint %}

### Current Gear

![](<../.gitbook/assets/image (25) (1) (1) (1).png>)

This section is exactly the same as the BIS Gear section, but instead represents the gear you currently have on the Job. This information will be important for the Team pages later.

### Filters

![](<../.gitbook/assets/image (11).png>)

This provides a simple way of narrowing down the options for Gear choices to a range of item levels. Whenever new raid tiers are added, the default options will be changed to the range of that tier, but you can change these to a range of values starting from 560.

### Actions Menu

![](<../.gitbook/assets/image (27).png>)

This set of buttons provides various features to help with creating and managing BIS Lists. Each button's function is outlined below.

#### Create / Save

This is the standard Create / Save button. Use this to save your information.

#### Create / Save and Sync Current Gear

![](<../.gitbook/assets/image (29).png>)

When pressed, this button will display a popup like the one above. This allows you to select other BIS Lists for the same job that, when you click the "Create / Save and Sync" button, will have their Current Gear set to be the same as the BIS List you are currently creating / updating.

#### Import

When the Extra URL field is filled in with a link to an [https://etro.gg](https://etro.gg) gearset, this button will become active, allowing you to import the data from it and populate the BIS gear section.

{% hint style="warning" %}
Please note that due to the fact Etro stores each individual item, and Savage Aim sticks to using general names for all classes, the import feature may not be 100% perfect every time.

The import system will find the most similar Gear name in the database for each item, and sometimes this algorithm may find closer names than expected.

If this happens, please let me know by visiting the Discord!
{% endhint %}

#### Load Current Gear

![](<../.gitbook/assets/image (26).png>)

Finally, this button allows you to populate the Current Gear section of the current BIS List with the Current Gear of a chosen other BIS List with the same Job.

Clicking one of the boxes in this popup will load the Current Gear from that BIS List into this one.

## Editing an Existing List

After clicking the create button when making a new list, or clicking one of your lists on the Character page, you will be taken to a similar page to before. However, there will be the data that you input previously already populating the inputs.

Also, the button at the bottom will say Save instead of Create, and the breadcrumb trail at the top will state the name of the Job the List is for, instead of saying "New BIS List".

## Character Page Display

If you return to your character's page, you will see that your lists have been added to the BIS List box, and should look something like this;

![](<../.gitbook/assets/image (18) (1).png>)

A full breakdown and explanation of this page is available on the next page!
