---
title: Sync Obsidian Vaults for Free
---




I am experiementing using obsidian as my writing tool for this digital garden. The problem i face is that i want to be able to sync my obsidian files across multiple devices. 

I followed  this how to guide by [Face Dragons](https://facedragons.com/foss/sync-obsidian-across-devices/) which allowed me to set up syncing across Macbook and android without having to subscribe to obsidian sync which costs $10USD pcm which seems a little too pricey at the moment. I may consider subscribing in the future to support the team. I'll review this in 3 months to make an assessment.

## Download Syncthing

Firstly you need to download [Syncthing](https://syncthing.net/downloads/) on each of the devices you want to use. for iOS users sorry you can't download Syncthing, and you need to either use icloud or google drive. I'm using an android phone and Syncthing is free and available on the google play store. 

### MacOs
Download Syncthing for Mac [here](https://syncthing.net/downloads/)

#### Android
Download Syncthing for Android [here](https://play.google.com/store/apps/details?id=com.nutomic.syncthingandroid)

#### iOS
😭 You can't download syncthing, there are alternative work arounds in the Face dragons article.

## Set up Syncthing on your primary device (mac)
Once you've downloaded the .dmg and installed it as usual, open the program, either from the toolbar, or by navigating to (http://127.0.0.1:8384/)

## Set up Syncthing on your secondary device
Connect your secondary device to your computer by clicking on "Add Remote Device" in the lower right corner. Make sure you have syncthing open on you secondary device as well! I found that to set this up correctly on Android, it required me to toggle into the Web UI mode from the app.

Before moving to the next step make sure the default sync folder is being shared between your devices

## Add your Obsidian vault to Syncthing
Click on "Add Folder'' and in the folder path navigate to your obsidian vault
Sharing Tab > share with your connected devices

## Connect the sync'd folder to Obsidian
Open Obsidian on your secondary device and choose the sync'd file as the vault

Thats pretty much it, it took me 20 minutes to do this and it updates really quickly 

Syncthing did not like markdown files ending with a '?' so i renamed those





