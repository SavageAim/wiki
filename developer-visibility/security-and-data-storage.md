---
description: Just a brief writeup for what I'm doing for data security
---

# Security and Data Storage

## What Data Is Stored

### Discord

Though Discord is used for login, there is nothing related to your Discord authentication stored in Savage Aim. When logging in for the first time, the backend (using [https://github.com/pennersr/django-allauth](https://github.com/pennersr/django-allauth)) stores the username and email address associated with the account. It is my interpretation that changing these will cause auth to create a new account.

### FFXIV

Savage Aim stores the Lodestone ID of Characters that are created in the system. When initially importing the Character, it also grabs the Avatar URL from the Lodestone which is how it displays the Character's portrait.

## How and Where Data Is Stored

Savage Aim is currently split over two separate servers. One is a front facing server running the website code. This is only accessible via the HTTP and HTTPS, and SSH connections using an SSH key are allowed so that I can deploy the new versions of the site.

The second server is completely isolated from the public network, and this is where our data is stored. This is an extra layer of protection to keep your data safe.
