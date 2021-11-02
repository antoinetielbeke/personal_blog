---
title: "Removing the Cloud connection from my 1st gen Xiaomi robot vacuum"
date: 2020-09-15T11:30:03+00:00
# weight: 1
# aliases: ["/first"]
tags: ["home assistant", "smart home"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: true
hidemeta: false
comments: false
description: "Hands-on with the new Slimme Lezer and HommeAssistant 2021.8.0 Energy update."
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
    image: "https://raw.githubusercontent.com/Hypfer/Valetudo/master/assets/logo/valetudo_logo_with_name.svg" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/<path_to_repo>/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---
When I still lived with my parents we had three dogs. I am a big animal lover and I love all of my dogs but my god they lose a lot of hair. Vacuuming daily became the norm because the other option was having a house covered in dog fur. This is the moment I convinced my parents to buy a robot vacuum. The Xiaomi Mi Robot Vacuum cleaner Gen 1. The machine was happily used (and abused) until January 2020 when I moved out of my parents house, then it was decided my parents would get a new vacuum robot and the Gen1 would go to his retirement home (my small apartment). The first thing that annoyed me is that all of my IoT was local and not Cloud connected *except* for my vacuum. This made me stumble onto the Valetudo project.

## What is Valetudo?
> Valetudo aims to be a vendor-agnostic abstraction and cloud replacement for vacuum robots which started as a standalone binary on rooted roborock vacuums.

## How to install Valetudo
First I always like to prepare a good workspace before I start something. Lets first create a new folder
``` bash
mkdir /valetudo
```
Since it is a Python project, we need to create a virtual environment. I like using PyEnv for all of my VirtualEnv but you can use whatever floats your boat.
`pyenv virtualenv 3.9.7 valetudo`
and now activate it!
`pyenv acticate valetudo`
Install the necessary packages
