<p align="center">
  <img src="http://soundcloud-dl.com/soundcloud-download-logo.png" alt="Logo"/>
</p>

# SoundCloud Music Downloader
## Python Version
* FlyinGrub has decided to **change the language**, because the bash one started to be a little too messy...
* He has choosen python cause it's nice, **simple**, efficient but more :
    * There is a lot of tool made by the community (like **eyed3**) that can be imported very easily
    * It allow an **easier installation**
    * It will be fully **compatible** with Linux/Os x/Windows without hacking (like previously for os x)
* It already fixes all the issues of the bash version and add others features.
* You can find it **[here](https://github.com/flyingrub/scdl)**

## Changelog : MUST READ !
* the .scdl.cfg has been changed a few time ago before reporting any issue be sure you have the latest one in your $HOME !!
* Please read the new instructions below, if you want to update/install/reinstall

## Description

This shell script is able to download music from http://www.soundcloud.com.
It should work with OS X, any Linux OS.

## System requirements

* Unix like OS with a proper shell
* Tools we use : `sed` ; `tr` ; `echo` ; `grep` ; `cut` ; `sort` ; `uniq`.


## Required tools

* You will need `eyeD3` ; `curl`
* Only OSX : `brew`


## Instructions

### Install :
1. Be sure that you have all the required tools.
2. `wget https://raw.githubusercontent.com/lyoshenka/soundcloud-dl/master/soundcloud-dl.sh && chmod +x soundcloud-dl.sh`

### Fire :
1. Type `scdl {OPTION} {URL}`
* For help type `scdl -h`

## OPTIONS available
* `-l [URL]       ` Use this Url. (Necessary, or pass the url as the first argument)
* `-o [OFFSET]    ` Begin the download with a custom offset.
* `-p [PATH]      ` Use a custom path for this time.
* `-c             ` Script will continue if a sound as already been downloaded.
* `-r             ` Download only the repost.
* `-d             ` Debug mode.
* `-h             ` Show this help.

## Features

* Automatically detect which kind of Soundcloud's link you have provided
* Download all song of an user's page
* Download all repost of an user's page
* Download all song of a song page
* Download all song of an user's playlist page
* Download all song of an user's list of playlist page
* Download all song of a group page
* Download all song of an user's liked song
* Set tags with eyeD3 (skip the tag if eyeD3 is not installed)
* The script stop when he see one song that is already downloaded
* You can use it as a sync script as i do with my Raspberry PI, each night it launch the script with my soudncloud and if new song has been reposted it download it and stop when it encounter a song that has already been downloaded.

## License

[GPL v2](https://www.gnu.org/licenses/gpl-2.0.txt), orignal author [Luka Pusic](http://pusic.si)
