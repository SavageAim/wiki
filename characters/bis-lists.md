---
description: All about the management of BIS Lists for Characters
---

# BIS Lists

## Tracking Gear

Once you have your Characters imported and set up, we can begin to track the Gear they have versus the Gear they need. To do so, we can create a new BIS List.&#x20;

After importing and verifying a Character, we should be on a page like this;

![](<../.gitbook/assets/image (10).png>)

To add a new BIS List, click the purple "Add New" button to the right of the BIS Lists box.

## Make a New List

You should have ended up on a page that looks like this;

![](<../.gitbook/assets/image (4).png>)

The form in its current state is quite large, and split into 4 sections; Details, BIS Gear, and Current Gear, which are the details required and maintained, and then a Filters section, which allows for filtering the gear in the dropdowns by a range of item levels. There is also a large green "Create" button at the bottom, which as the name suggests, will create the new List once ready.

### Details

![](<../.gitbook/assets/image (6).png>)

In the Details section, you can pick the Job associated with the list, and optionally add a URL. The URL can be to sites like etro and ariyala and while Savage Aim cannot currently import lists from these sites, it could be helpful to have an easy link to an external site as well.

{% hint style="info" %}
Currently, due to having to figure some things out, you can currently only track one BIS List per Character per Job. This is something that should be dealt with in the near future, but you can check the [dev-roadmap.md](../dev-roadmap.md "mention") to see how progress is going.
{% endhint %}

### BIS Gear

![](<../.gitbook/assets/image (17).png>)

This section of dropdowns allows you to pick the Best in Slot gear for the List. The options in the dropdowns are the various types of Gear you can acquire, filtered for what can be equipped in that slot.

{% hint style="info" %}
For any job other than Paladin, the "Off Hand" option will not be available to choose. This is because only Paladin currently has the option to have different types of item in the main and off hand slots.
{% endhint %}

### Current Gear

![](<../.gitbook/assets/image (25).png>)

This section is exactly the same as the BIS Gear section, but instead represents the gear you currently have on the Job. This information will be important for the Team pages later.

### Filters

![](<../.gitbook/assets/image (3) (1).png>)

This provides a simple way of narrowing down the options for Gear choices to a range of item levels. Whenever new raid tiers are added, the default options will be changed to the range of that tier, but you can change these to a range of values starting from 560.

{% hint style="warning" %}
There is currently a minor bug with this where it can remove already chosen options if the filters make the items go out of range. This will be fixed soon.
{% endhint %}

### Saving

Once you've filled out all your details for the list, click the create button. If all is successful, you should see a green notification pop up, and the page will change to the edit version of the same page, for the new list you just made.

If any errors occur, the appropriate inputs will be marked in red and have text displayed next to them informing you of the error.

## Editing an Existing List

After clicking the create button when making a new list, or clicking one of your lists on the Character page, you will be taken to a similar page to before. However, there will be the data that you input previously already populating the inputs.

Also, the button at the bottom will say Save instead of Create, and the breadcrumb trail at the top will state the name of the Job the List is for, instead of saying "New BIS List".

## Character Page Display

If you return to your character's page, you will see that your lists have been added to the BIS List box, and should look something like this;

![](<../.gitbook/assets/image (21) (1).png>)

This darker box is a link to your BIS List's edit page. It shows the Job icon and name on the left, and on the right will be a little tag that indicates two things.&#x20;

Firstly, the colour of the tag will be blue, green, or red, depending on if the Job is a Tank, Healer, or DPS.&#x20;

Secondly, the number in the box displays the _current_ item level of the list. That is to say the item level of the gear you currently have equipped according to this list. This should match what the game tells you.
