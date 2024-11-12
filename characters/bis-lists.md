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

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

The form in its current state is quite large, and split into 5 sections; Details, BIS Gear, and Current Gear, which are the details required and maintained, and then a Filters section, which allows for filtering the gear in the dropdowns by a range of item levels. Lastly there is a small section with a couple of Create / Save buttons.

On mobile, the form is split into tabs, and should look something like the below picture when you first load in. The tabs on mobile correspond with the sections above, but keep the mobile UI easier to use!![](<../.gitbook/assets/image (21).png>)

The Actions section will be displayed below each tab for ease of use.

### Details

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

In the Details section, you can pick the Job associated with the list, and optionally add a URL and a name.&#x20;

#### Name

An optional name for the BIS List. This will be used in places to potentially differentiate between different BIS Lists for the same job.

Names are used in the [character-details.md](character-details.md "mention") page, as well as the [#bis-list](../teams/create-a-team.md#bis-list "mention") part of the Join Team, Create Team, or Edit Team Membership pages.

#### Job

The Job for which the BIS List is for. Used to display Job icons in various places and also to determine whether Offhand should be tracked separately for Paladins.

#### URL

A URL to any site you want. A link will be displayed under BIS List cards to this website, and is handy to have for easy access to sites like Etro where materia information is stored alongside gear.

{% hint style="info" %}
If you insert an Etro Gearset URL, you will be able to import the BIS Gear straight into Savage Aim as well! See [#import](bis-lists.md#import "mention") for more details.
{% endhint %}

### BIS Gear

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

This section of dropdowns allows you to pick the Best in Slot gear for the List. The options in the dropdowns are the various types of Gear you can acquire, filtered for what can be equipped in that slot.

{% hint style="info" %}
For any job other than Paladin, the "Off Hand" option will not be available to choose. This is because only Paladin currently has the option to have different types of item in the main and off hand slots.
{% endhint %}

#### Import from Etro

The "Import from Etro" button located at the bottom of the card is how you can import your BIS data from the link you provide in [#url](bis-lists.md#url "mention"). If a valid [https://etro.gg](https://etro.gg) link is present in this input, the button will instead look like below, and clicking it will attempt to run an import against the given URL.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Please note that due to the fact Etro stores each individual item, and Savage Aim sticks to using general names for all classes, the import feature may not be 100% perfect every time.

The import system will find the most similar Gear name in the database for each item, and sometimes this algorithm may find closer names than expected.

If this happens, please let me know by visiting the Discord!
{% endhint %}

#### Import from XIVGear

Similarly to the above, SavageAim also supports importing gearsets from XIVGear.app. if a valid [https://xivgear.app](https://xivgear.app) URL is provided, then the button will change to the following;

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

Unlike Etro, XIVGear provides the ability to store multiple sets per sheet, and generate a URL that contains multiple sets. When a URL like this is used, the page will prompt you with a popup to decide which one to select. Clicking on one of the names will import that set.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Please ensure to select either "Link to Whole Sheet" or "One Link for Each Set" when exporting from XIVGear to import into SavageAim!
{% endhint %}

### Current Gear

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

This section is exactly the same as the BIS Gear section, but instead represents the gear you currently have on the Job. This information will be important for the Team pages later.

#### Import from Lodestone

This button will attempt to import whatever gear is currently equipped to your character as per their Lodestone page, and set the values of your "Current" gear to whatever it finds.

It will only work if the gear worn by your character as per the Lodestone is equippable by the Job that the BIS is currently set to. If it is not, it will give an error message instead of changing the Job for the list.

{% hint style="warning" %}
Also note that similar to Etro imports, there is a level of name matching that may not always be 100% accurate!
{% endhint %}

#### Copy from Other List

![](<../.gitbook/assets/image (26) (2) (1).png>)

Finally, this button allows you to populate the Current Gear section of the current BIS List with the Current Gear of a chosen other BIS List with the same Job.

Clicking one of the boxes in this popup will load the Current Gear from that BIS List into this one.

If there are no other BIS Lists for the chosen Job, the button will be white and unclickable instead.

### Filters

![](<../.gitbook/assets/image (3) (3).png>)

This provides a simple way of narrowing down the options for Gear choices to a range of item levels. Whenever new raid tiers are added, the default options will be changed to the range of that tier, but you can change these to a range of values starting from 560.

### Create / Save Buttons

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

There are two buttons that can be used to Create / Save BIS Lists. The top is just a simple Create / Save button which will Create a new BIS List, or Save the changes you made to an existing one.

#### Create / Save & Sync Current Gear

![](<../.gitbook/assets/image (29).png>)

When pressed, this button will display a popup like the one above. This allows you to select other BIS Lists for the same job that, when you click the "Create / Save and Sync" button, will have their Current Gear set to be the same as the BIS List you are currently creating / updating.

If you have no other BIS Lists for the chosen Job, then this button will instead be black and will not do anything when pressed.

## Editing an Existing List

After clicking the create button when making a new list, or clicking one of your lists on the Character page, you will be taken to a similar page to before. However, there will be the data that you input previously already populating the inputs.

Also, the button at the bottom will say Save instead of Create, and the breadcrumb trail at the top will state the name of the Job the List is for, instead of saying "New BIS List".

## Quick Set to BIS

<figure><img src="../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

In situations where you have non-BIS Current Gear, and you want to quickly update your item to BIS without having to go through a whole dropdown to get there, we've added a new button on the Current side to quickly update your Current item for the slot to be BIS.

The button will appear in any circumstance where the Current item for a slot does not match the BIS item.

## Character Page Display

If you return to your character's page, you will see that your lists have been added to the BIS List box, and should look something like this;

![](<../.gitbook/assets/image (18) (1) (2).png>)

A full breakdown and explanation of this page is available on the next page!
