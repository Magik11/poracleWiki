---
title: Profiles
nav_order: 3
layout: default
parent: English
grand_parent: User Guide
---

# Profiles
Profiles allow you to specify different tracking configurations for different times.
You create profiles with `!profile add` eg `!profile add home`.  You can list your profiles with `!profile list`

Note that to change tracking switch to a particular profile (eg `!profile home`, issue tracking, location or area commands and these will be set to the current profile.

But what about automatic change based on time of day?  You can do 
`!profile settime` _activationtimes_ - where the activationtimes are 
days of week & times to activate - eg 'mon9:15' or 'weekday17:00' or 
'weekend09'.  

Every 10 minutes Poracle will check if a profile was due to activate and will set it.

`!profile add <name>`
This will add a new profile with the name provided. If you currently have no profiles then your current !tracked settings will be applied to this profile. If you have an existing profile then this command will create a blank profile. If you want to copy the settings from one profile to another then use the `!profile copyto <name>`.

`!profile <name>`
This will switch to the profile with the name provided.

`!profile copyto <name>`
This will copy the profile settings of the currently selected profile to the profile name provided.

`!profile list`
This will list the available profiles, displaying which is currently selected with an asterisk (*) by the number associated with the profile as well as when the profile becomes active.

`!profile settime <timestring>`
This will apply a time setting to the current profile for when this profile will become active. Change to a different profile with `!profile <name>' to apply time settings to a different profile.

`!profile rename <name>`
This will remove a profile of the name provided.
