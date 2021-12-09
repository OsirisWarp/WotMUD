# WotMUD
Scripts and other documents for Wheel of Time MUD primarily for the Mudlet client

Currently using the fantastic pack Adael as built (https://github.com/weisluke/WoTMUD) as a base for all additional work. Most current project is color coding items to determine rough value. See below for examples, this should not be counted as 100% accurate as item values and worth change.


# Item Quality

This package adds coloured tags to the end of the most commonly used weapons and armour. This is not an exhaustive list, but is designed to help newer players (and myself) in determining what may be worth picking up and what can be left on the group. Depending on your build, playstyle and preference the value you place on each item may vary to other players. These values are intended as a quick guide to help when looking for new gear, it is expected for you to also do further research.  Some items that are valuable may also not be listed. If you come across any of these please let me know so I can add them in.

A few rare or unique items are also missing long descriptions (decription on the ground) if you come across any of these items please send me the long description so I can add it.
I will try to keep the values updated based on any nerfs or big changes to items. 

Clan trinkets still need to be done, but most other items of worth have now been added. 
Categories set as Abs, Combo, Dodge, Shield and Everything for armor and trinkets. Weapons are set to their weapon category. 
Colours Tiers are Magenta > Orange > Purple > Blue > Green

In general newer players will want to be aiming for purple weapons with a mix of Orange, Purple and Blue armor and trinkets. 
I would recomend turning these triggers off when in PK, they should not add much load as they are just adding text. But they may slow you slightly if multiple triggers are having to fire. The package can be enabled using syntax: _enablequal_ and disabled with _disablequal_

Some example pictures: 

<img src="https://user-images.githubusercontent.com/71254862/145162379-2dc33bc4-9057-42c5-b8df-4fac813efe3b.png" width="15%"></img> 
<img src="https://user-images.githubusercontent.com/71254862/145162388-c7473e07-193f-4967-836f-657c60d8de3b.png" width="15%"></img> 
<img src="https://user-images.githubusercontent.com/71254862/145162394-e855a48a-6080-41d0-b924-4e1c2afa9a31.png" width="15%"></img> 

# Travel Weave

This is my travel scripts, I'm sure there is a much better way to do this but I went with a qucik and dirty option just to get it rolling. As such please use at your own risk and be sure to look at how this is working so you can prevent any accidents. Usage is simple with the _setports_ being used while in Tar Valon, this then captures locations around Tar Valon and saves them for later.  

The first dangerous part comes in to the fact that port codes expire at month reset. This is somewhat mitigated by checking the previous month when using the _time_ command, and if the month changes while logged in by triggers reacting to the month change message. In general it is best practice to use the _setports_ command when first logging in to ensure codes at the most up to date. 

To use these codes there are two methods, F1 is bound a quick port to TV. This can simply be deleted from the keys section of Mudlet if you have no use for it. For me it is a quick easy way to get back to TV and also useful in an emergency as it's a single button press. 

The other way is to use the command _travel_ followed by the location (TV, Cairhien, Caemlyn, FD or WB) currently this is case sensitive and has to be exactly this for it to go to the correct location. I will be updating this shortly to not matter for case sensetivity and also allow for short or full names of cities.
This is the second dangerous part of the package, currently if you enter travel orange it will use orange as the port code.

I have this set for me personally so I can simply type travel and then copy and paste a port code from a locate object or locate life search. However, if you are not careful this can lead to accidently trying to travel to somewhere you don't want. For example in it's current state if you use "travel caemlyn" it won't take you to the caemlyn saved port code. It will use the word caemlyn as your port code and thus have undesired effects. 

## PLEASE TAKE CARE WHEN USING THIS TRAVEL SCRIPT

I will work to safe proofing this further in the future, currently using it for myself more than others. But with sharing it I will work to make sure it's safe for those using it.
