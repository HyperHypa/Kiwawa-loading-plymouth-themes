<h1 align="center">Kiwawa Loading Plymouth Themes</h1>

**************

![gif](sample1.gif)

### How does this project work?

This project uses [Plymouth](http://www.freedesktop.org/wiki/Software/Plymouth) to create an eye-candy splash screen to boot screen that shows after you select the kernel to boot into and displays the animation until your login manager shows.

### What is [Plymouth](http://www.freedesktop.org/wiki/Software/Plymouth)?

[Plymouth](http://www.freedesktop.org/wiki/Software/Plymouth) is an application that runs very early in the boot process that provides a graphical boot animation while the boot process happens in the background. 

### How do I install this theme?

1. Check if you have Plymouth installed.
```bash
# If running this command shows "Unknown command: plymouth", you do not have plymouth installed.
# Check the frequent questions section on how to install Plymouth.
plymouth
```
2. Move into a suitable place to temporarily install the theme. This can be wherever you want, but I would recommend doing this in the Downloads folder.
```bash
# Move back to the Home directory.
cd

# Move into the Downloads directory.
cd ./Downloads
```
3. Clone the theme.
```bash
git clone https://github.com/HyperHypa/Kiwawa-loading-plymouth-themes.git
```
4. Place it into your Plymouth theme folder.
```bash
# Copy the the file into the Plymouth theme folder. 
cp -r ./Kiwawa-loading-plymouth-themes/Kiwawa-loading /usr/share/plymouth/themes/

# Check if theme was successfully copied into the directory. There should now have "Kiwawa-loading" among the list of themes.
sudo plymouth-set-default-theme -l
```
5. Set the default theme to "Kiwawa-loading"
```bash
# This command should set the theme if there are no errors shown.
sudo plymouth-set-default-theme -R Kiwawa-loading
```
Your job is done, try rebooting the system to see if it works.

## FAQ

### 1. How do I install Plymouth?

Try searching on YouTube with the prompt "How do I install Plymouth on ***WhateverDistroYouUse***", they will explain it 100 times better than I could.

### 2. Does this work on Windows?

No. If you know how to do so without messing with the bios, I'd love to learn how you do it.

### 3. Will you add this onto the AUR?

This would depend on if I have the time to learn it.

### 4. Can you help me install it?

Ehhhh maybe? The instructions are up if you want to get this Plymouth theme working. If there are any issues with the instructions, feel free to make a pull request for it.