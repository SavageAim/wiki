---
description: Change some settings on the site!
---

# User Settings

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

The User Settings page allows control over certain User specific details on the site. The different sections are outlined below.

{% hint style="info" %}
Any tab with unsaved changes will have their name marked with an asterisk (**\***).
{% endhint %}

## User Details

The User Details tab allows you to edit your username, but it's left open to extend to more if people have any ideas!

### API Key

In an effort to extend the functionality of the site to be open to external features (did someone say Dalamud Plugin?), we now support users creating an API Key. This API Key can be used to interact with the API as a User.&#x20;

Clicking the "Generate API Key" button will replace the button with a display that looks like this;

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If anyone wants to create any extra tool/suite/etc to use/extend the SavageAim API, the API Key should be passed as `Authorization: Token <api_key>` in the headers of HTTP Requests.\
\
Also if you do end up making something with this, feel free to post it in the Discord and we can also feature it somewhere!
{% endhint %}

## Colour Scheme

<figure><img src=".gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

This setting is used to control the colours used on the [#character-cards](teams/team-overview.md#character-cards "mention"). The dropdown at the top provides a list of the themes currently supported in the system. The choice is rendered in the table below, as a method of indicating what the chosen theme looks like.

{% hint style="info" %}
Only this table updates live, to update other tables you will need to save first.
{% endhint %}

If you want to submit your own colour scheme suggestion, something can be organised, but throw up an issue on the Github Repo if you can! One helpful tool I like to use is [https://vis4.net/palettes/#](https://vis4.net/palettes/), using 7 colours!

{% hint style="info" %}
The "Explanation of Colours" card below is an expandable card that gives the new explanation of what the colours mean. This used to be accessible as a popup in the navbar, but it was moved here to clean up clutter.
{% endhint %}

## Notifications

![](<.gitbook/assets/image (45).png>)

This panel controls the Notifications you will receive in the system. Individual types of Notifications can be turned off and on as required, so you have full control over what types of events you will be informed of.

{% hint style="info" %}
For full details on the Notifications in the system, check [notifications.md](notifications.md "mention")!
{% endhint %}

## Loot Manager Version

![](<.gitbook/assets/image (46).png>)

This page allows you to pick between the Per Item Loot Manager ([loot-tracker.md](teams/loot-tracker.md "mention")) or the new Per Fight Loot Manager ([per-fight-loot-manager.md](teams/per-fight-loot-manager.md "mention")).&#x20;

## Loot Solver Settings

<figure><img src=".gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

This section allows you to change settings related to the [loot-solver.md](teams/loot-solver.md "mention"). Currently the only setting you can edit is its greediness.

The Loot Solver running in Greed-y mode will make it so it stops assigning items as soon as everyone can buy their last remaining augment token (or item in the case of the first floor).  This allows you to start assigning items for alternative BIS Lists slightly faster.

It is freely toggleable, and will not break your current Loot Solver predictions to turn it on / off as you see fit!
