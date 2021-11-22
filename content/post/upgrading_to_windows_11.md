---
title: "Upgrading to Windows 11, my way"
date: 2021-11-14T11:30:03+00:00
# weight: 1
# aliases: ["/first"]
tags: ["windows", "backup"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: false
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "How I upgraded from Windows 10 to Windows 11 while keeping all my personal files."
# canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
cover:
    image: "/img/upgrading_to_windows_11/windows_11_logo.jpg" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: false # only hide on current single page
editPost:
    URL: "https://github.com/<path_to_repo>/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---
Now that Windows officialy released Windows 11 for more than one month, I feel safe to upgrade my personal desktop. After years of upgrading my own, my family and friends desktops I feel like I found the most comfortable way to upgrade your Windows system.

It looks something like this:
1. Back-up all my personal files (excluding installed software)
2. Create a Windows 11 USB
3. Nuke my main drive with Windows 10 and install Windows 11 from the USB
4. Restore all my personal files (excluding installed software)
5. Install all the software that I need (manually)
6. Done!

**ACKNOWLEDGEMENT** 1. Whenever I say "all of your personal files" I mean all of the diretories that are specified in your File History settings. 2. I am not responsible for any lost files, programs or whatever ;)  

## 💾 Backing up all personal files with Windows File History
- not perfect back-up solution
- Prefer veeam endpoint backup
- perfect for upgrading though

Open "File History or access it through the controlpanel with the following path: `Control Panel\All Control Panel Items\File History`
Click Select `Select drive` and your avaiable disks for file history will show up. In my case, I have a NAS so I added it by clicking `Add network location`. 

![selecting your network drive in file history](/img/upgrading_to_windows_11/select_network_drive.png#center)

After I selected the drive I want to use for File History, it immediately starts backing up your personal files. This might take a while (for me, 300GB took about 2-3 hours).

![bla](/img/upgrading_to_windows_11/network_drive_selected.png#center)


## Creating the Windows 11 USB
I will not go too deep into explaining how to do this because there are plenty tutorials for this online. My preferred way is to use the [Windows Media creation tool](https://www.microsoft.com/en-gb/software-download/windows11). It formats the USB and throws a bootable Windows 11 installation on it. Double-triple-check if you REALLY made a file history back-up, shutdown your PC and boot up from the USB.

## Installing Windows 11 and nuking my disk

## ↩️ Restoring my personal files
Open up File History and on the left menu click on `Restore personal files`. A new window will pop up and here you can see all of the folders on your back-up. Check if you have the most recent back-up (date is in the left top) and click on the big green restore button.

![restore_files](/img/upgrading_to_windows_11/restore_files.png#center)
It will ask you if you want to replace the files in the destination, click on `Replace the files in the destination`.
![replace_file](/img/upgrading_to_windows_11/replace_files.png#center)
This might take a while, I had 300GB to transfer so it took about 2 hours.

## Final words
Now you have a clean Windows 11 setup with all of your personal files! 
