---
layout: page
title: Create Question - MR Card Game
description: A Mixed Reality-Based Card Game for Formal and Informal Education.
sitemap:
    priority: 0.7
    lastmod: 2022-11-29
    changefreq: weekly
---

## Create Your Own Quiz

In this page, you will learn how to create your own quiz using our question creator, which can be found [here](https://github.com/KritiaSthovania/MR-Question-Creator-For-Card-Game). The created quizzes, which are stored in a single folder, should be then uploaded to a remote source for in-game download or you can also directly copy it into the corresponding folder, see the `Setup` page for more detail.

### Main Menu

If you want to create new quizzes, you should click the `Create Exercise` button; if you want to modify questions of an existing quiz, you should click the `Browse Directories` to select the folder and question file.

<div><a class="image main"><img src="{{ "/images/Creator_Home.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Create New Quiz

After choose the question you want to modify or clicked the `Create Exercise` button, you will see the panel where you can add or modify questions as the image below.

<div><a class="image main"><img src="{{ "/images/Create_Question.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

Before adding a question, you must first create an empty folder for the quiz by clicking the `Browse Directories` button on the top right and then the `Create directory` button. Then you also need to give a description. The root folder is the **MyDocument/MRQuestion Creator/levelSave** folder, e.g. **User/Documents/MRQuestion Creator/levelSave** under Windows. Then you need to specify the type of question, *Multiple Choice* or *Input*, and if you want to add an image to the question, click on the empty filed under the `Question Image` label on the top left part. Then, a window will show up which require you to specify the **Web URL** of an image, ending with *.jpg* or *.png*, other format cannot be recognized. By clicking the `Import` button, the specified image will be downloaded and shown the the filed. If you want to change the downloaded image, just click the filed again and then click `Delete`.

<div><a class="image main"><img src="{{ "/images/Import_Image.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>
<div><a class="image main"><img src="{{ "/images/Image_Added.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

Click the `Add` button to formulate the question. Click `Create` to save it.

<div><a class="image main"><img src="{{ "/images/Add_MC.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

If you imported an image, the image will be automatically linked to this question and be deleted in the field. Then you can start to add another question.

### Modify/Add Questions

To add new questions to an existing quiz, just select a folder using the `Browse Directories` button on the creator panel and then follow the instructions in the `Create Question` secton. If you want to modify a question, instead of selecting a folder, you need to select the question. Then, the question name will appear on the bottom right part. Clicking the question name to open the *Creator Panel* with its existing information. Note that if you want to change or delete the image of an existing question, you still need to first click the name to open the *Creator Panel* so that the image can be loaded to the corresponding field. At last, click the `Change` button. The image below shows you the panel after specifying and clicking on an exising question with its image.

<div><a class="image main"><img src="{{ "/images/Modify_Question.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

**Important: you must click on the `Save` or `Apply Change` button at the bottom right corner to finalize the whole process, otherwise there might be some unexpected error.**

### Upload Quiz

The upload function under the `Browse Directories` on the home menu is not applicable, so you must manually do that. The questions are saved in the folder named as the quiz's name. Their names are `QuestionXXX.json` and their images are named as `QuestionXXX_image.jpg/png`. You just need to copy the whole directory under the corresponding folder introduced in the `Setup` page. After that, enjoy your game!