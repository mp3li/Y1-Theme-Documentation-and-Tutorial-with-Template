![Innioasis Y1 / Theme Documentation and Tutorial](https://img.shields.io/badge/Innioasis%20Y1-Theme%20Documentation%20and%20Tutorial-8A2BE2?labelColor=2E2E2E)
![Skill Level / Complete Beginners to Advanced Users](https://img.shields.io/badge/Skill%20Level-Complete%20Beginners%20to%20Advanced%20Users-8A2BE2?labelColor=2E2E2E)
![Features / Every Single Theme Option](https://img.shields.io/badge/Features-Every%20Single%20Theme%20Option-8A2BE2?labelColor=2E2E2E)
![Development / Active](https://img.shields.io/badge/Development-Active-8A2BE2?labelColor=2E2E2E)

# Y1 Theme Documentation and Tutorial for Beginners

This documentation reflects everything currently known and tested about Innioasis Y1 theming. As theme development evolves, the Y1 firmware updates, and new discoveries are made, this guide will continue to be updated. This documentation and tutorial are actively maintained resources.

This documentation and tutorial may not be hosted or shared elsewhere, in whole or in part, and may only be hosted on mp3li official channels. For business inquiries please contact mp3li via official channels such as Github, Patreon, Reddit, or TikTok (socials in bio and bottom of this documentation).

This documentation and tutorial was initially posted on my Patreon for free and paid members only, and is now public on Github and Patreon. 

----

### How Themes Actually Work:

Y1 themes are shockingly simple! It’s just a folder with pictures and one file that tells the Y1 what each image is used for. 

Think of the Y1 like this:
It opens a folder, looks for a file called config.json, reads what it says, and then loads the images you tell it to load.

So instead of thinking “I’m coding a theme,” think:

“I’m organizing a little art folder and giving the Y1 a map.”

This guide is long, but don’t let that scare you away. The main reason it’s long is because there’s truly so many things you can do to your themes and I go over every single option. This guide is beginner friendly and if anyone has any questions at all or needs help, feel free to reach out.

If you used this guide in any way to create a theme, please give this repo a star and consider a shoutout to mp3li’s theme creating guide in your social media post and/or description where people download it! 

----

### What this Guide Contains + Table of Contents:

<details>

<summary><em>Open What this Guide Contains + Table of Contents:</em></summary>

<br>

- [Simple, beginner-friendly and easy to understand explanations on how the Y1 themes work](#how-themes-actually-work)

- [What each theme option in the config file actually means in simple terms, in nine sections](#what-every-theme-setting-actually-means)

- [Beginner-friendly explanations on how to use each theme option](#what-every-theme-setting-actually-means)

- [Minimum required files for a working theme](#minimum-required-files-for-a-working-theme)

- [Theme folder structure](#theme-folder-structure)

- [Simple steps on how to create your own custom theme by editing an existing theme and how to properly attribute](#how-to-edit-an-existing-theme-and-how-to-properly-attribute)

- [Simple steps on how to create your own custom theme from scratch](#how-to-create-a-theme-from-scratch)

- [Tips on what file type, sizes your images can be, and color format](#tips-on-file-type-image-sizes-and-color-format)

- [Tips on being safe with license files, for example when you use pop-culture images that you do not own](#tips-on-being-safe-with-license-files)

- [Why your theme might not be showing up or loading correctly + technical rules for the config file](#technical-rules-for-the-config-file--why-your-theme-might-not-be-showing-up-or-loading-correctly)

</details>

----

### How this Guide is Different from the Other Theme Documentation:

There is already a detailed and technically thorough theme guide in the community, created by a developer whose work I respect. That documentation is an excellent resource for users who want a deeper, more technical view of how the system works.

This guide is meant to complement it, not replace it. 

While exploring the themes that ship with the Y1, I noticed that the system is really flexible with the way themes are put together. For example, some things that are often thought as required are actually optional, and theme files can be organized in different ways as long as the file paths are in the config file. This means you can name files anything you’d like, you don't have to put everything in one folder, and you can organize files however you prefer and use as many folders as you’d like in your themes.

----

### Why I Made this Documentation and Tutorial:

I wrote this documentation after directly testing stock Y1 themes and building multiple high quality [themes of my own](https://www.patreon.com/collection/1908526?view=expanded) that utilize every single theme feature.

This guide is being created because I care deeply about bridging the gap between non-tech-savvy users and technology itself. 

Using my background in software development, I thoroughly looked into the original Y1 themes to fully understand them in order to create my own themes. I created this guide months ago for myself and use it (alongside other tools I will also be releasing in the near future) to make my themes. And now that I’ve gained a shocking amount of members in just a month, I want to give back directly to you all with this theme documentation so you all can make your own beautiful themes too. I am keeping this post for free and paid members only temporarily, and soon I will also unlock it for non-members and also post it on GitHub. But for now, this is a thank you to you all. 

My goal is that everyone is able to make themes to the device’s fullest capabilities. 

This guide aims to make sense to both those who have absolutely no idea what they're doing, and those who do. 

----

### What Every Theme Setting Actually Means:

In this section I'll be going over a theme config file that comes on the Y1 when you first get it, section by section and explaining what 100% of the things actually mean and how they're used in this format:

Theme option name in simple terms: Easy to understand description of what that theme setting is, does, and/or means

The actual line in the config file

---

### Section 1 of 9: Theme Info

<details>

<summary><em>Open Theme Info:</em></summary>

<br>

Theme title: the name of your theme

"title": 

Theme author/creator: who made the theme

"author":

Theme author/creator URL: Link to anywhere that is yours. Could be social media, github, a personal website, etc 

"authorUrl": "",

Theme description: Write a description for your themes

"description":

</details>

---

### Section 2 of 9: General Theme Settings

<details>

<summary><em>Open General Theme Settings:</em></summary>

<br>

Theme Cover: The little image for the theme when you're scrolling through all your themes while choosing one on the device 

"themeCover":

Theme Color: I honestly have not seen this setting actually affect anything on the device itself, but it is there as an option so I am continuing to look into it and still wanted to include it here

"themeColor":

Theme Text Color: This is the only other setting I have not seen actually affect anything on the device itself, and for this one too I am continuing to look into it and wanted to include it here

"themeTextColor": 

Desktop Wallpaper: This is the wallpaper for your main menu screen only 

"desktopWallpaper":

Global Wallpaper: This is the wallpaper for your now playing screen and your list screens

"globalWallpaper":

Desktop Mask: This image layers on top of your main menu screen, can be used for additional details, and is not required

"desktopMask":

Font: This is the theme for your font and must be a .ttf file. You can convert .otf font files to .ttf using free in-browser converters

"fontFamily": 

</details>

---

### Section 3 of 9: Main Menu Screen Theme Settings

<details>

<summary><em>Open Main Menu Screen Theme Settings:</em></summary>

<br>

There are 11 main menu icons.

Now Playing Icon: This is your now playing icon on your main menu screen

"nowPlaying":

Music Icon: This is your music icon on your main menu screen

"music": 

Video Icon: This is your video icon on your main menu screen

"video": 

Audiobooks Icon: This is your audiobooks icon on your main menu screen

"audiobooks": 

Photos Icon: This is your photos icon on your main menu screen

"photos": 

FM Radio Icon: This is your FM radio icon on your main menu screen

"fm": 

Bluetooth icon: This is your bluetooth icon on your main menu screen

"bluetooth": 

Settings Icon: This is your settings icon on your main menu screen

"settings": 

eBook Icon: I've never seen this actually on the device, but it's promising that it's included in their themes!

"ebook":

Calculator Icon: I've never seen this actually on the device, but it's promising that it's included in their themes!

"calculator":  

Calendar Icon: I've never seen this actually on the device, but it's promising that it's included in their themes!

"calendar":

</details>

---

### Section 4 of 9: List Settings

<details>

<summary><em>Open List Settings:</em></summary>

<br>

There are two sections of list settings. One applies to the main menu list, and the other applies to lists in the list screens. You can either utilize this to make the two lists look different, or make them match for cohesiveness.

Main Menu List Settings:

 Unselected List Item Text Color: This is the text color of unselected list options

"itemTextColor":

Selected List Item Text Color: This is the text color of the selected list item

"itemSelectedTextColor": 

Image Behind Selected List Item: This is the wide and short rectangle image behind the selected list item

"itemSelectedBackground": 

Image Behind Unselected List Item: This is the wide and short rectangle image behind the unselected list item, leave blank for none

"itemBackground":

Arrow: This is the tiny icon on the right end of your selected list item

"itemRightArrow":

---

### List Screens Settings:

List Screen Background Color: This is the color of the background of the list area

"menuBackgroundColor":

Image Behind Unselected List Item: This is the wide and short rectangle image behind the unselected list item, leave blank for none

"menuItemBackground": 

 Unselected List Item Text Color: This is the text color of unselected list options

"menuItemTextColor": 

Image Behind Selected List Item: This is the wide and short rectangle image behind the selected list item

"menuItemSelectedBackground": 

Selected List Item Text Color: This is the text color of the selected menu item

"menuItemSelectedTextColor": 

</details>

---

### Section 5 of 9: Now Playing Screen Settings

<details>

<summary><em>Open Now Playing Screen Settings:</em></summary>

<br>

Progress bar text color: The color of the ‘0:00’ numbers on the now playing screen 

"progressTextColor":

Progress bar color: The color of the progress bar (the portion you’ve already listened to) on the now playing screen

"progressColor": 

Progress bar background- The color of the progress bar (the portion you haven’t listened to yet) on the now playing screen, leave blank for none

"progressBackgroundColor":

</details>

---

### Section 6 of 9: Folder View Settings

<details>

<summary><em>Open Folder View Settings:</em></summary>

<br>

Folder icon image: The tiny icon image to the left of every folder in folder view 

"folderIcon": 

Music icon image: The tiny icon image to the left of every music file in folder view 

"musicIcon": 

</details>

---

### Section 7 of 9: Status Bar Settings

<details>

<summary><em>Open Status Bar Settings:</em></summary>

<br>

There are 18 status bar icons.

All top status bar icons can be left blank in the config if you would like to not use any top status bar icons, besides Play, Pause, and Stop.

Currently playing music icon: The tiny icon in your status bar that only appears when music is currently playing 

"playing": 

Currently playing audiobook icon: The tiny icon in your status bar that only appears when an audiobook is currently playing

"audiobookPlaying": 

Currently playing FM radio icon: The tiny icon in your status bar that only appears when FM radio is currently playing

"fmPlaying": 

Currently stopped audio icon: The tiny icon in your status bar that only appears when any kind of media is currently stopped

"stop": 

Paused icon: The tiny icon in your status bar that only appears when any kind of media is currently paused

"pause": 

Bluetooth currently connected icon:

"blConnected": 

Bluetooth in process of connecting icon: The tiny icon in your status bar that only appears when Bluetooth is in the process of connecting 

"blConnecting": 

Bluetooth is disconnected icon: The tiny icon in your status bar that only appears when Bluetooth headphones have disconnected 

"blDisconnected": 

Headset with mic icon: The tiny icon in your status bar that only appears when headphones with a microphone are connected 

"headsetWithMic": 

Headset without mic icon: The tiny icon in your status bar that only appears when headphones without a microphone are connected 

"headsetWithoutMic": 

Battery icons (low to full): These are your battery icons, listed from low to full, including charging versions. I've left the input (strings, for the technical folks) empty for these so you can see how they're structured:

"battery": [

    "",

    "",

    "",

    ""

],

"batteryCharging": [

    "",

    "",

    "",

    ""

]

Status bar color: This is the color of your upper status bar

"statusBarColor":

</details>

---

### Section 8 of 9: Setting Screen Settings

<details>

<summary><em>Open Setting Screen Settings:</em></summary>

<br>

There are 49 settings screen icons. 

Setting mask: You can use this for either overlay effects that overlay on top of your desktop background, or use this to set an entirely individual settings screen wallpaper

"settingMask": 

Shutdown icon: This is your shutdown icon on your settings screen 

"shutdown": 

Timed shutdown icons: These are your timed shutdown icons, ranging from off to 120 minutes before shutdown on your settings screen, the numbers represent minutes

"timedShutdown_off": 

"timedShutdown_10": 

"timedShutdown_20": 

"timedShutdown_30": 

"timedShutdown_60": 

"timedShutdown_90": 

"timedShutdown_120": 

Shuffle on and off icons: These are your shuffle on and off icons

"shuffleOn": 

"shuffleOff": 

Repeat off, repeat all, and repeat one icons: These are your repeat off, repeat all, and repeat once icons

"repeatOff": 

"repeatAll": 

"repeatOne":

Equalizer icons: These are your equalizer icons

"equalizer_normal": 

"equalizer_classical": 

"equalizer_dance": 

"equalizer_flat": 

"equalizer_folk":

"equalizer_heavymetal": 

"equalizer_hiphop":

"equalizer_jazz":

"equalizer_pop": 

"equalizer_rock": 

Key lock on and off icons: These are your key lock on and off icons

"keyLockOn": 

"keyLockOff": 

Key tone on and off icons: These are your key tone on and off icons

"keyToneOn": 

"keyToneOff":

Key vibration on and off icons: These are your vibration on and off icons

"keyVibrationOn":

"keyVibrationOff": 

Wallpaper icon: This is your icon for the change wallpaper feature on the settings screen

"wallpaper": 

Backlight icons: These are your backlight icons - the numbers mean seconds, always means always on

"backlight_10": 

"backlight_15": 

"backlight_30":

"backlight_45": 

"backlight_60": 

"backlight_120":

"backlight_300": 

"backlight_always": 

Brightness icon: This is your brightness icon

"brightness": 

Display battery on icon: These are your display battery on and off icons

"displayBatteryOn": 

"displayBatteryOff": 

Date & time icon: This is your date and time icon

"dateTime": 

Language icon: This is your change language icon

"language": 

Launcher icon: This is a rockbox/launcher toggle, but I have never seen it on the device, if someone has I would love to know!

"launcher": 

Factory reset icon: This is your factory reset icon

"factoryReset": 

Clear cache icon: This is your clear cache icon

"clearCache": 

Change theme icon: This is your change theme icon

"theme": 

File extension on icon: This is your file extensions on and off icons

"fileExtensionOn": 

"fileExtensionOff":

</details>

---

### Section 9 of 9: Dialog (Pop-Up) Settings

<details>

<summary><em>Open Dialog (Pop-Up) Settings:</em></summary>

<br>

Dialog option background: This is the color of the rectangle of the unselected dialog option 

"dialogOptionBackground": 

Dialog option text color: This is the text color of the unselected dialog option

"dialogOptionTextColor":

Dialog option selected background: This is the background of the selected dialog option

"dialogOptionSelectedBackground": 

Option selected text color: This is the text color of the selected option text

"dialogOptionSelectedTextColor":

Pop up dialog background color: The background color of the dialog pop up

"dialogBackgroundColor":

Dialog text color: The text color of the upper text of the dialog 

"dialogTextColor": 

</details>

---

### Minimum Required Files for a Working Theme:

<details>

<summary><em>Open Minimum Required Files for a Working Theme:</em></summary>

<br>

<a id="minimum-required-files-for-a-working-theme"></a>

I have been playing around with leaving things out of a theme and trying it on my Y1, and it seems like the Y1 will replace any missing needed files with a standard default file. For example, a cover image is not required because the Y1 will fill in an empty theme cover with a default standard cover image. From what I can tell, and if I learn I am mistaken I will update this guide, is that you cannot 'break' a theme by leaving anything out. 

Required files for a working theme:

A config.json file

Any files that you are referencing in the config.json file is ideal, but if you leave out any assets (assets = any files in your theme, like images, fonts, everything) the Y1 will insert a default asset in any missing asset's place

</details>

---

### Theme Folder Structure:

<details>

<summary><em>Open Theme Folder Structure:</em></summary>

<br>

<a id="theme-folder-structure"></a>

While exploring the themes that ship with the Y1, I noticed that the system is really flexible with the way themes are put together. For example, some things that are often thought as required are actually optional, and theme files can be organized in different ways as long as the file paths are in the config file. This means you can name files anything you’d like, you don't have to put everything in one folder, and you can organize files however you prefer and use as many folders as you’d like in your themes.

A large amount of themes currently have all of their theme files in one singular folder. For my themes, I organize all assets in a variety of folders to help me find what I'm looking for and make creating themes as smooth and simple as possible. If you'd like to make editing an existing theme that has everything combined in one singular folder significantly easier, you could check out the config file for the theme and see what each image is used for and put them in folders to organize them. If you do this, you must update the file path in the config file, and it's very easy. The file path always assumes you are already in your main theme folder.

For example: 

"nowPlaying": "nowplayingicon.png" 

If you put it into a folder called main menu Icons, it would turn into...

"nowPlaying": "main menu icons/nowplayingicon.png" 

I've put assets behind up to 5 or 6 folders, and that is absolutely not the limit. As long as you tell the config file where to find the file by giving it the file path, everything works great. 

Config files must go in the root folder, meaning they must be inside the main theme folder and cannot be behind any additional folders.

Theme folders can be organized however you would like, as long as the config file is in the main theme folder, and you specify the file path(s) in the config file. 

</details>

---

### How to Edit an Existing Theme and How to Properly Attribute:

<details>

<summary><em>Open How to Edit an Existing Theme and How to Properly Attribute:</em></summary>

<br>

<a id="how-to-edit-an-existing-theme-and-how-to-properly-attribute"></a>

To edit an existing theme, first download it from whichever source it may come from. 

The simplest and easiest way to edit an existing theme is to choose and find your own files to replace existing files with. Then, you would copy/paste or drag/drop the new file(s) to the same folder as the file you're replacing, and rename the new file with the name of the file you are replacing. This works because the config is looking for that specific file name in that specific place.

Or, if you'd like to make editing an existing theme that has everything combined in one singular folder significantly easier and more organized, check the section above called Theme Folder Structure for more information. If you prefer the more organizational method, you can rename files to anything you would like, and organize them in any folder structure you like, as long as you specify file paths in the config. 

#### When to attribute someone else's work: 

If you build a theme completely from scratch, no credit to the original theme author is needed

If you start with a theme that you did not make and edit it in any way (images, layout, config, asset set, structure, etc.), then attribution is required

This isn’t about owning characters or source art — it’s about crediting the theme package itself as the starting point (the layout, configuration, curated assets, and how it’s assembled to work on the Y1).

For example, the icons in most creators' themes aren’t just pulled from Google Images — they’re edited, resized, cropped, and sometimes padded by the theme creator so they display and align correctly on the Y1. The same goes for backgrounds, spacing, and how everything is mapped in the config. When those pieces are reused at all, as a set, or starting point, that’s considered building on the original theme.

Meaning, you cannot take the photo files other creators have chosen, edited, and resized, in any way shape or form for your theme without attribution. Even if you only use just a few of the icons from someone else's theme for example, that is still using icons from their theme, and requires attribution. Taking directly from someone else's theme package is not the same as going and finding the original source yourself, and editing it yourself. Just because a creator uses an asset that is easy to find on Google, does not mean you can use their exact file from their theme package and put it into yours with no attribution. 

If you do not want to attribute credit, do not use any files that directly came from someone else’s theme. Using even just 10% of anyone else’s theme content requires attribution. 

You can absolutely still say the theme is by you. 

Attribution just means acknowledging what it was built from.

Nobody wants to see someone else using their work and passing it off online as 100% their own creative work. This is illegal due to license files, and is not the standard to set for the theming community. If you made a wholly original theme, wouldn’t you want someone to credit you if they used any part of it? 

#### How to Credit (Examples):

You can phrase it however you like! Here are a few easy formats, where either the theme you used as a base or the theme creator is filled into the blanks:

"Based on the ______ theme by  ______" 

"Edited from a _____ by ______"

"Remix of ______ by ______"

"Icons reused from ______ by ______." 

"Some icons reused from ______."

"Battery icons credit goes to ______." 

If you’re sharing the files, it is also a suggestion to either keep or update the author and/or description field in the config to reflect that it was modified from someone else's original theme. (That requirement is in my license files, for my themes). 

Why this Matters

Attribution is standard practice in creative and developer communities. It helps people trace where things came from, gives credit to the original work, and keeps the ecosystem healthy and respectful as it grows. 

And just like you, I hold myself to these same standards. If I was to remix someone else’s theme I would follow these same guidelines.

</details>

---

### How to Create a Theme from Scratch:

<details>

<summary><em>Open How to Create a Theme from Scratch:</em></summary>

<br>

<a id="how-to-create-a-theme-from-scratch"></a>

To create a theme from scratch, first you make a folder for the theme and name it anything you would like. Then, you decide if you want everything all in one folder, or if you want to organize things. Either way provides the same end result. 

If you'd prefer a more organized method, the folder structure that I use for my own themes is below. Using this folder structure is not required in any way, and is only included as an example that you are welcome to adopt in your own themes. If you do not prefer this method, all you need is your one theme folder and you can skip ahead.

Inside the main theme folder:

config.json file

backgrounds folder

font folder

main menu icons folder

all other images folder

assetbank folder

Inside assetbank folder:

used folder

unused folder

Inside all other images folder:

folder view folder

status bar folder

settings menu folder

Inside folder view folder:

folder icon folder

music icon folder

Inside status bar folder:

audiobook playing folder, paused folder, bluetooth connected folder, stopped folder, fm radio playing folder, top status bar folder, battery copy folder, bluetooth disconnected folder, headphones without mic connected folder, bluetooth connecting folder, music playing folder, battery folder, headphones with mic connected folder

Inside settings menu folder:

key tone on off folder, date and time folder, file ext on off folder, repeat folder, change theme folder, display battery on off folder, clear cache folder, shutdown folder, equalizer folder, shuffle on off folder, arrow folder, mini settings folder, wallpaper mini icon folder, language folder, brightness folder, backlight folder, behind selection folder, timed shutdown folder, shuffle quick folder, key vibration on off folder, factory folder, key lock on off folder

Then you must make the file your Y1 will use to know how every asset will be used on your Y1's screen: the config.json file. A config.json file must be a plain text file. It cannot be a Word document, Google Doc, or PDF renamed to .json. The file must be inside the main theme folder, and it must be named exactly: config.json 

On Windows:

Open Notepad

Paste or type your config content

Click File → Save As

Change “Save as type” to All Files

Name the file config.json

Make sure it does not say config.json.txt

On Mac:

Open TextEdit

Click Format → Make Plain Text

Paste or type your config content

Click Save

Name it config.json

Make sure it does not add .txt

After creating your config.json file, you can plug your Y1 into your computer and copy and paste the stock theme folder Melody Muncher onto your computer. This theme uses all config options available. Then you can use use the stock theme config as a template by copy and pasting the contents into your own config file and deleting the filled out parts, resulting in a blank config file ready to be turned into your own theme. 

Make sure to check the info in all other sections of this documentation + tutorial for more specifics, like what each line in the config means, how to format the config, tips for file types and image sizes, and more. 

</details>

---

### Tips on File Type, Image Sizes, and Color Format:

<details>

<summary><em>Open Tips on File Type, Image Sizes, and Color Format:</em></summary>

<br>

<a id="tips-on-file-type-image-sizes-and-color-format"></a>

File Types:

Image files:

All image files must be .png format (background images, icon images, etc.) 

Images can include transparency wherever you'd like, not just the outer areas

The config file must be a .json file

Font files must be a .ttf file. You can convert .otf fonts to .ttf fonts online for free using in-browser converters

Color Format:

Colors in the config file are written using hex color codes.

The most common format looks like this: “#RRGGBB”.

For example, “#FF0000” is red, and #FFFFFF is white

You can also include transparency by using this format: “#AARRGGBB”.
The first two characters control how transparent the color is.
For example, “#80FF0000” is red with about 50 percent transparency.

If you are not sure what hex code to use, most built-in computer photo editors and many in-browser photo editors have a color picker tool. This tool lets you click on any color on your screen and it will show you the exact hex code for that color. It's a very easy way to grab specific colors from wallpapers, icons, or other images you are using in your theme

Image sizes:

Main menu screen icons and settings screen icons: 

There is no set required size or aspect ratio required for icons

The stock main menu screen and settings screen icons tend to be around 166px by 166px, but I've made mine 500x by 500x, and then I stopped adding extra transparent padding to make them perfectly square because it's unnecessary. Then I stopped resizing them all to the same size in general because I noticed the Y1 automatically scales all assets to fit the Y1's constraints. Be mindful of image size though, as larger than needed images both takes up precious space on your Y1 and can also make your theme more likely to crash your Y1. No damage will be done to your device or theme, but keeping things generally small is the best practice. Some of my icon sizes are: 600px by 729px, 794px by 1321px (this one is on the larger size and I should probably downsize it, this size is for an unreleased theme icon), and 350px by 500px, for example. I have tested themes with various asset sizes on three separate Y1 devices with no issues

Rectangle(s) behind selected and unselected list items:

640px by 91px

The stock themes use rectangle images that are colored either solid or transparent hex colors, in the size listed above. I personally have not tested other sizes/aspect ratios, because sticking to this same rectangle size has been simple

Wallpaper(s)

640px by 480px 

The stock themes use wallpaper(s) with the above size. I bet it's possible to use bigger images as long as they're the same aspect ratio, but I have not tried. I simply edit any image I would like to be a theme background image to have the above aspect ratio/size and try to be mindful of how large my asset sizes are

Tiny icon next to selected list item:

There is no set required size or aspect ratio required for the tiny icon next to your selected list item

The stock themes use an image sized 64px by 64px

For my own work, I typically use an image sized roughly the same as my icons for my tiny icon next to the selected list item. I noticed that manually sizing down any image that small often ruined the quality, and I really wanted that image crisp. The Y1 automatically scales assets to fit in the space they go in on the device screen

Status bar icons:

There is no set required size or aspect ratio required for status bar icons

The stock themes use images that range from 225px by 225px, to 480px by 223px

For my own work, I typically use an image sized roughly the same as my icons for a few of my status bar icons. Like above, I noticed that manually sizing down any image that small often ruined the quality, and I really wanted that image crisp. The Y1 automatically scales assets to fit in the space they go in on the device screen. For some of my status bar icons, I recolor ones included in stock themes. For my status bar icons, I drew my own custom set and I recolor them for each theme I make

</details>

---

### Tips on Being Safe With License Files:

<details>

<summary><em>Open Tips on Being Safe With License Files:</em></summary>

<br>

<a id="tips-on-being-safe-with-license-files"></a>

This community thrives on fan made themes. A lot of themes are inspired by media, games, brands, and pop culture. We all love these themes so much and love seeing more and more of them made every day. Handling this responsibly is key, so we remain a safe space for fan work.

Always include a LICENSE.txt or CREDITS.txt file inside your theme folder. Even if your theme is free. Even if it feels obvious. This makes your intent clear and protects you.

In your license file:

State that the theme is fan made

State that you do not own any copyrighted characters or brands used

State that the theme is not affiliated with or endorsed by the original creators

Clearly credit any artists if you used fan art with permission

Do not claim ownership of characters, logos, or brands that are not yours. 

If you plan to monetize themes, be especially careful. Original artwork is always the safest long term option.

Strong license files protect you, protect the community, and show professionalism. When everyone includes clear credits and disclaimers, it helps keep fan creativity alive without causing unnecessary problems. 

</details>

---

<a id="technical-rules-for-the-config-file--why-your-theme-might-not-be-showing-up-or-loading-correctly"></a>

### Technical Rules for the Config File + Why your Theme Might not be Showing up or Loading Correctly:

<details>

<summary><em>Open Technical Rules for the Config File + Why your Theme Might not be Showing up or Loading Correctly:</em></summary>

<br>

When the Y1 loads a theme, it simply reads the config.json file. If something in that file is written slightly wrong, even something small like it has a comma in the wrong place or is missing a comma, the device can’t understand it and will act like you did not drag and drop that theme onto your device.

Here’s what usually causes that: 

The file name needs to be exactly config.json in all lowercase. If the file is accidentally saved as config.json.txt or anything similar, the Y1 won’t be able to recognize it

The config.json file should live directly inside your main theme folder, not inside another folder

The config file needs to be plain text. If it was made in Word or Google Docs and then renamed, it won’t work. It has to be created in a plain text editor

Inside the file, the formatting matters. JSON requires quotation marks around both the setting name and the value. For example:

"title": "My Theme",

Without quotation marks around My Theme and title, it won’t load

Brackets matter too. Your entire config file starts with an opening curly bracket { and ends with a closing curly bracket }. Every time you open a new section like "itemConfig": { you must close it with a matching }. If one bracket is missing, the Y1 cannot read the file at all

Commas are also important. If there’s another line underneath, the line above it needs a comma. But the very last line in a section should not have a comma

Correct example of comma and bracket use:

{
"title": "My Theme",
"author": "Your Name"
}

Incorrect example with an extra comma at the end:

{
"title": "My Theme",
"author": "Your Name",
}

The config.json file also uses square brackets [ ], which mean you are listing multiple things in order. On the Y1, this is used for things like battery icons. For example:

"battery": [

    "battery_low.png",

    "battery_half.png",

    "battery_threequarters.png",

    "battery_full.png"

],

That list is an array. Think of it like a row of items lined up in order. The Y1 reads them from top to bottom:

First image = lowest battery

Second image = next level

Third image = next level

Fourth image = full battery

The order matters. If you accidentally rearrange them, your battery levels will look wrong on the device. Very important rules about arrays:

They start with [ and end with ]

Each item inside must be in quotation marks

Each line must have a comma except the last one

If you forget a bracket, the entire theme will not load

There is also a separate array for charging battery icons, using the same idea and same rules:

"batteryCharging": [

    "charge_low.png",

    "charge_half.png",

    "charge_threequarters.png",

    "charge_full.png"

]

If square brackets feel scary, just remember:

Curly brackets group settings. Square brackets list multiple files in order. That’s it.

Empty Strings: Some assets can be purposefully left out and will not be automatically replaced with a Y1 default asset, and the area they go in will remain blank. This can be used as a style choice or to make extra simple themes. In the config, that looks like this:

Correct: "itemBackground": ""

Incorrect: "menuItemBackground":

Those two quotation marks with nothing inside are called an empty string. An empty string tells the Y1 “I’m not giving you a custom image or color here." This is different from deleting the line completely. In this guide I specify what assets can be left blank, without automatically being replaced by a default asset

File names also need to match exactly. If the config says Music.png but the file is named music.png, the Y1 sees those as different because it's case-sensitive. The config.json file is also case-sensitive  

Most loading issues come down to one of these small formatting details, and below includes specific issues and their solutions

I don't see my theme on my Y1's theme list screen: if your theme doesn't appear on your list of themes on your device, it is most likely because of a formatting error in the config.json file. Read the above information in this same section for how to resolve this issue

My theme font doesn't show up on my Y1: if your font doesn't appear on your Y1, it is most likely either because of a formatting error in the config.json file, or because the font is not the compatible file type. The required file type for fonts is .ttf. If you want to use an .otf file you can use free in-browser .ttf to .otf converter websites

I don't see the colors I chose for my theme on my Y1: if your chosen colors for your theme don't appear on your device, it's most likely either because of a formatting error in the config.json file such as the hex color is too short/has a typo, or possibly trying to choose a color for a setting that can only accept an image

I don't see the images I chose for my theme on my Y1: if your chosen images don't appear on your device, it's most likely either because of a formatting error in the config.json file, because the image is too big, or the wrong file type. All image files must be .png files

</details>

---

### Note from the Dev:

If anyone has any questions at all or needs help, feel free to reach out 🫶🏻

If you used this guide in any way to create a theme, please give this post a like and consider a shoutout to mp3li’s theme creating guide in your social media post and/or description where people download it! I hope you all create amazing themes using this documentation and tutorial. Feel free to share anything you've created with me, I'd love to see! 
