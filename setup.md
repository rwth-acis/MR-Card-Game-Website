---
layout: page
title: Setup - MR Card Game
description: A Mixed Reality-Based Card Game for Formal and Informal Education.
sitemap:
    priority: 0.7
    lastmod: 2017-11-02
    changefreq: weekly
---

<!-- Text stuff -->

## How to Setup the Game

### AR Image Targets
To play the MR Card Game, printing out the AR Image Targets is required. These are physical card that you can find here. Simply download and print out the sheet in this .pdf-file and cut out the individual cards with scissors or a different cutting device. The "board" card is only a placeholder. 

<div> <ul class="icons alt">
			<li><a href="https://github.com/rwth-acis/MR-Card-Game/raw/main/Image%20Target%20Pictures/Image%20Targets%20Printed.pdf" class="button icon fa-download">Image Targets</a></li>
	  </ul>
</div>

### Quizzes
In order to play the MR Card Game, you will also need pre-build quizzes from which the questions are asked during the game. You can create this quiz by yourself using the MR Card Game Question Creator Tool which you can download [here](https://github.com/rwth-acis/MR-Question-Creator-For-Card-Game). You can find a tutorial for creating quizzes on the `Create Quiz` page above. You can also simply download a pre-built quiz in the app, these quizzes are stored [here](https://github.com/rwth-acis/MR-Card-Game-Quizzes). Simply select `Download Levels` in the Main Menu and click on any of the quizzes that interest you. They are immediately downloaded and ready to play in the `Play Levels` section in the Main Menu.

After creating or downloading a quiz, the quiz folder has to be placed on your device in the following folder (Application.persistentDataPath):
- **Android:** `\Card\Android\data\com.RWTH-ACIS.MRCardGame\files\` 
- **Windows:** `C:\Users\USERNAME\AppData\LocalLow\RWTH-ACIS\MR Card Game`

This is important otherwise the quiz won't show up in the app. If you downloaded the quiz through the game, they are automatically stored properly.

If you want to link your remote source folder (e.g. a GitHub repo) to the download functionality in the game, you need to clone the repository and manually change the `Request Base URL` field expired on the inspector of `DownloadLevels` script which you can find in the `Hierarchy` of the `IntroScene` under `Canvas/Panel/BackgroundBrowseDirectories/DwonloadLevelsMenu`. Specifying a URL directly in the game is not supported yet.



