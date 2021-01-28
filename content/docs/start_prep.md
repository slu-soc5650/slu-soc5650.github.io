+++
title = "Preparing Your Computer"

date = 2018-12-04T00:00:00
lastmod = 2021-01-26T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
# weight = 1

# Add menu entry to sidebar.
linktitle = "Computer Prep"
[menu.docs]
  parent = "Getting Started"
  weight = 7
+++

## Overview
Before you begin the semester, there are a number of things that you should do to help set yourself up for success. **All of the applicable sections below should be completed before our first class on February 1st.**

<br>

## Computer Prep
Please work through the following steps:

1. Make sure your operating system is up-to-date. If you are able, I would also recommend upgrading your computer to the most recent release of its operating system that the computer can run.
    - On macOS, you can do this through the [App Store](https://support.apple.com/en-us/HT201541). *The one exception is upgrading to Big Sur. I have not yet done so and, if you have not either, I recommend holding off. I will not be testing out our course materials with Big Sur this semester.*
    - Both [Windows 7](https://www.dummies.com/computers/computer-networking/network-security/how-to-manually-check-for-windows-7-updates/) and [Windows 10](https://support.microsoft.com/en-us/help/4027667/windows-update-windows-10) have system update tools, though if you have Windows 7, you should consider upgrading to Windows 10.

2. We'll be sharing computer files throughout the semester, so you should ensure that you have functioning anti-virus software and that it is up-to-date.

3. You'll also need to download files, so you'll need to make sure you have at least **twenty gigabytes** free if you are not. If you're not sure how to check this, here are some instructions for [Windows](https://www.lifewire.com/how-to-check-free-hard-drive-space-in-windows-2619187) and [macOS](https://www.macworld.com/article/2972775/os-x/how-to-check-your-macs-free-hard-drive-space.html).
    - Options for de-cluttering include deleting files that are no longer needed, moving files to an external device, moving files to a cloud storage system, or upgrading the internal hard drive (may not be possible for macOS users and some Windows users).

4. Make sure you know how to access your computer's file management system.
    - On macOS, this means being comfortable with Finder.app for finding folders, making new ones, and opening files. Here are some tips for using Finder on recent versions of [macOS](https://support.apple.com/en-us/HT201732).
    - On Windows, this means being comfortable with Windows File Explorer for finding folders, making new ones, and opening files. Here are some tips for using File Explorer on [Windows 7](https://www.dummies.com/computers/operating-systems/windows-7/how-to-navigate-windows-7-with-windows-explorer/) or [Windows 10](https://www.dummies.com/computers/operating-systems/windows-10/how-does-file-explorer-work-in-windows-10/).

<br>

## R
### Base R
You can download `R` from its [website](https://cloud.r-project.org). Choose "Download R for (Mac) OS X" or "Download R for Windows". Windows users should look for text that says "install R for the first time" and click the `base` to the left of that text. Both macOS and Windows users should install `R` version 4.0.3, known as "Bunny-Wunnies Freak Out" (`R` version nicknames come from [Peanuts](https://livefreeordichotomize.com/2017/09/28/r-release-names/)).

If you already have `R` installed, please make sure you have the latest version. You can upgrade it using the same process for a new installation.

### RStudio
RStudio is a graphical user interface for `R` that will make learning the language and using it much, much easier. You should download the *free* version of RStudio from [their website](https://www.rstudio.com/products/rstudio/download/#download). Choose the appropriate installer for your platform. Make sure `R` is already installed before installing RStudio. 

If you already have RStudio installed, please make sure you have the latest version. You can upgrade it using the same process for a new installation.

### R Packages
The packages we will need this semester can be downloaded using the following code chunk in RStudio's console:

```r
install.packages(c("tidyverse", "here", "janitor", "knitr", "leaflet",
  "mapview", "measurements", "naniar", "RColorBrewer", "remotes", "rmarkdown",
  "sf", "testDriveR", "tidycensus", "tigris", "tmap", "viridis", "webshot"))
```

You should only have to run this once per computer. If you are not sure where to find the console, don't worry - we'll talk about this on the first day of class!

### PhantomJS
PhantomJS is a means for creating "headless" web-browsers and thus rendering the output of HTML widegts in `knitr` documents. It makes it possible to get a screengrab of a `leaflet` map when you "knit" your `.Rmd` files, for instance. To install it, use the following code chunk in RStudio's console:

```r
webshot::install_phantomjs()
```

Like installing packages, you should only have to run this once per computer. Again, if you're not sure about using the console, don't worry - we'll talk about this on the first day of class!

<br>

## Get Started with GitHub
The service that is hosting this website is called [GitHub](https://github.com/). GitHub is used by programmers, data scientists, and researchers for hosting computer code, data, and project materials (like websites). We will be using GitHub extensively this semester. You will need a free account, which you can sign up for one from GitHub's [homepage](https://github.com/). If you already have a GitHub account, you do not need a new one. 

Once you have a GitHub user name, send Chris an email with it so that you can be added to the [SOC 4650 & SOC 5650 organization](https://github.com/slu-soc5650). After you have been added to the organization, you should find your assignments repository and check the **Issues** tab. There should be an open **Issue** describing how feedback will be disseminated this semester. Please read it and then *close the issue* so that we know you've seen it.

<br>

## GitHub Desktop
In addition to the applications above, everyone will need a local installation of GitHub Desktop, which is a graphical user interface for accessing Git and GitHub.com. It can be downloaded for free from the [application's website](https://desktop.github.com). You will need to download and run the installer. Once it is complete, you will need to login to the application with your [GitHub.com username and password](/docs/onboarding). 

