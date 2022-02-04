---
description: What comes next for Savage Aim
---

# Dev Roadmap

{% hint style="danger" %}
This page now only contains big missing chunks of functionality that are in my head as needed for the 1.0 release. For all other plans, please check the Trello board. It gives more information in a much nicer format than this!

[https://trello.com/b/elTOXk1W/savage-aim](https://trello.com/b/elTOXk1W/savage-aim)

Once 1.0 has been released I will likely remove this page in favour of just linking to the Trello!
{% endhint %}

Below is a list of items I want to work on, in order of priority. You can skip this page if you're looking to get into the helpful part of the Wiki.

A Trello board maintaining more granular information is available at [https://trello.com/b/elTOXk1W/savage-aim](https://trello.com/b/elTOXk1W/savage-aim)

## Live Notifications

Given the nature of Savage Aim, with Teams of multiple Characters belonging to multiple people, I feel like it's worth having some sort of notification system in place for live updates.

For some examples, notifying when a verification request has been completed, or failed, and some information about it.

It will also be helpful in the next big update in notifying people of changes that were made by someone else.

## Deleting Objects

I've left this out of the current app for now for a valid (in my opinion anyway) reason.

The handling of deleting objects needs to cascade in the correct way and I wanted to sit down and have the chance to think about that and only that at a later point.

For example, deleting Characters would need to either update or delete Teams, BIS Lists etc.

Deleting a Team would need to notify people that it happened (see above).

Kicking members from a team, or leaving a team yourself, would be important places to start. They're relatively easy and don't affect too much.&#x20;

But I want to have notifications set up first.

To go hand in hand with this addition, I intend to make it so you can request to regenerate a Team's invite code so that if you need to kick people from a Team you can change the invite code to a new one.
