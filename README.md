# Edge Mimicry - Tree Style Tab Theme (Beta)
A theme created for Tree Style Tab extension on Mozilla Firefox, that tries to replicate the vertical tab user interface of Microsoft Edge Browser

![ezgif com-gif-maker](https://user-images.githubusercontent.com/81744148/154884867-e68a3464-cc64-4e65-bea1-b84822579d46.gif)

## Previews:
![ss-01](previews/SS-01.png) ![ss-02](previews/SS-02.png)
![ss-05](previews/SS-05.png) ![ss-06](previews/SS-06.png)
![ss-06](previews/SS-07.png) ![ss-07](previews/SS-08.png)



## Features include:
- support tab indention (up to 8 levels) [this restriction will be removed soon since I found a workaround on the theming and can finally support the built-in auto tab-idention]
- support for tab-coloring based on its container
- follows your current firefox theme
- built to handle different Firefox Sidebar configurations (so you can still use your own mods on userChrome without having to worry on breaking things on the tree style tab, well theoretically though if these mods are just as simple as changing the width, height, background etc. since I have no idea what kind of mods you've done on your userChrome sidebar.)

## How to install:
1. You must have [Tree Style Tab](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/) extension installed on Firefox.
2. Go to Firefox Add-Ons Manager > Tree Style Tab > Options , then click the :ballot_box_with_check: Unlock Expert Options.
3. On the Appearance section of the options page, choose the **"No Decorations"** to disable the built-in theme applied.
4. Scroll down on the options page until you find the "► Advanced" section and expand it. You will see a textfield there with a caption on the top **"Extra Style rules provided by Tree Style Tab"**.
5. Copy the entire code/content of the **treestyletab-edge-mimicry.css** and paste it on the textfield.
6. Close then open the sidebar to restart the tree style tab extension and to be able to load the theme correctly. Alternatively, you can also disable then enable the extension for it to properly load the css codes (and probably to reset the script handling for the pinned tabs, because there seems to be a problem with the pinned tabs layout when in "icons only" mode.)  

## Optional userChrome.css mods
If you want to also copy the hover feature of sidebar found on Microsoft Edge, then you can use the userChrome.css and other files included on the "edge-mimicry" folder. However, this sidebar mod will remove the resizeable feature since it uses a fixed width configuration.
## How to install userChrome.css mods (Windows):
1. You must have **toolkit.legacyUserProfileCustomizations.stylesheets** set to **true** on the **about:config** of Firefox. If you have not, then set it and restart firefox afterwards.
2. Launch the Run command window (Win Key + R) then enter **%appdata%**. From there, Navigate to Mozilla > Firefox > Profiles > bunch-of-random-strings-or-text-named-folder > chrome. If you cannot find the folder named "chrome", then create one.
3. Copy-paste both **userChrome.css** and the "edge-mimicry" folder on the "chrome" folder.
4. Re-launch Firefox.


## Important Notes:
- **For now it's still in beta again, because it seems that it doesn't work properly on some (or probably most) users as there seems to be problems with the icons. I am still working on to fix some issues, both on Windows and Linux Firefox platforms. Rest assured I'll update this repo once I'm done."
- When pasting the code to **Extra Style Rules**, make sure to check the **"No Decorations"** on Appearance panel option as this theme doesn't go well with the built-in themes of Tree Style Tab.

## Notes/Credits:
- Some of my userChrome mods were originally forked from [MrOtherGuy's Collection of random CSS hacks for Firefox](https://github.com/MrOtherGuy/firefox-csshacks), specifically the [autohide_sidebar](https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/autohide_sidebar.css) and implemented my own mods to it.
