# NoSplashTexts

## What?
The (hypothetically) multiversion solution to BlockyRick's Minecraft 1.17 resource pack of a similar name.

Original inspiration: https://www.planetminecraft.com/texture-pack/no-splash-texts/

## Who?
This is a solo project by me inspired by BlockyRick's past work.

## Why?
Sometimes, the splash texts by Mojang just won't fulfill your sense of humor. And sometimes, you just want to see that damned yellow text gone. But lo and behold, Mojang has a failsafe for intentionally blank `splash.txt` files (which is what BlockyRick's original pack did) and simply loads the text `missingno` if the `splash.txt` file is empty. See below for a demonstration:

![image](https://i.imgur.com/UOfiO.png)

(Source: https://imgur.com/UOfiO)

## How...

### ...do I install it?

Drop the `.zip` file into your resources packs folder, have it selected (as in, it should be on the right column in the resource pack menu), and **__reload your game__**.

(Optional for those playing on 1.14 and higher: The Fabric-based mod named "No Resource Pack Warnings" by SpaceWalkerRS — https://github.com/SpaceWalkerRS/no-resource-pack-warnings/releases)

### ...does this work?

A look inside the assets folder of this resource pack shows that it takes advantage of Minecraft's desire to render all formatitng codes possible. One of them, the obfuscator formatting code (`§k`), renders any character in equal width as the original character in question (from the Minecraft Fandom Wiki):

> The random characters placed after `§k` are always the same width as the original characters. For example, any random character cycled through where the letter "m" would be wide characters while any random character in the spot of an "i" would be narrow characters.

By not supplying any characters after the `§k` formatting code at all, Minecraft effectively renders no characters. Combine that factor with there being only one line in the `splashes.txt` file, and Minecraft is effectively trapped in rendering nothing for the splash text in the main menu regardless of the game version you're on. No need to run into the dreaded `missingno` text or instances of dated humor... yay!

(This means that until Mojang changes how formatting codes work—and it probably won't with a game this old and a feature this far cemented within Minecraft's history—this pack should work across all Minecraft versions that has `splashes.txt` support.)

## Where...

### ...are the demonstrations?

1.8.9:
![image](https://media.discordapp.net/attachments/728977460737081454/988446944051478558/2022-06-20_09.42.40.png)

1.18.2:
![image](https://i.imgur.com/aosY4X3.jpg)
