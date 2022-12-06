---
layout: page
title: How to Play the Game - MR Card Game
description: A Mixed Reality-Based Card Game for Formal and Informal Education.
sitemap:
    priority: 1.0
    lastmod: 2022-12-01
    changefreq: weekly
---
## How to Play the Game
After successfully starting a game as described in the `Play Levels` section, the game begins with the setup phase.

### Game UI
On the in-game UI you will see the starting `Currency` of 150. Players can use this currency to buy towers, traps and spells in the game. The `Wave` counter will also be visible and currently set to 0 as no wave has been started yet. With the start of each wave this counter will increase. Right next to it you can find the `Start next wave` button which upon being pressed, will start the next wave. After starting a wave, the `Start next wave` button will turn into an `Enemy` counter in the form of *enmemies died/total enemies*, which tells you how many enemies are in this wave in total and how many have been killed or reached the castle. You can find it in the other images on this page. Clicking on the `More Options` button, a scroll window will show up as seen in the image below. There are three additional buttons. By clicking on the `Lock Gameboard` button, you can disable the *Ground Plane* feature so that the position of the game board is locked (See the *Game Board* section). The `Refill Spell Deck` allows you to manually refill the spell (see the *Spell Cards* section). The `Return` button allows you to close this scroll window. Lastly, there are two small round buttons on the top right corner. The `cross` allows you to give up and return to the main menu. The `play` allow you to pause and continue the game at any time.
<div><a class="image main"><img src="{{ "/images/GameOverlay.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Game Board
<div><a class="image main"><img src="{{ "/images/BoardAxisTransparent.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

To start, you must first place the game board somewhere. The game enables the **Ground Plane** function of the underlying [Vuforia Engine](https://library.vuforia.com/), which means that the camera automatically searches a plane as the *Ground Plane*. After finding such a plane, a "dotted" square will show up as seen in the image, by clicking on the square, you can place the game board on the plane. Note that due to the limitation of the recognition functionality of the Vuforia Engine, the game board might not have a proper scaling sometimes. You need to move your smartphone here and there to get a appropriate size. It might be a little bit tricky so you need to try on your own. If you are satisfied with the placement, you can click on the `Lock Gameboard` button introduced in the `Game UI` section. Then, the **Ground Plane** function will be disabled and the game will stop trying to find planes, and the square will also disappear so that you don't need to worry about misclicks anymore. Of course, you can click on the button at the same place again to enable the funcion, which is called now `Unlock Gameboard`. 

The game board consists of many components. The castle that is connected to the stone path is your main base of defense. This is also the target you have to protect from the invading enemies. Every time an enemy enters the castle, the castle will take damage depending on the enemy's type. The castle's health is displayed above it as a green bar whose red part will grow as it takes damage. The total HP depends on the number of questions in the quiz. The stone path, which the castle is connected to, is the invading path of the enemies. They will spawn at the Portal placed opposite of the castle and walk (or fly) all the way around the woods in the middle along the stone path to reach the castle. But while they are moving toward the castle, they are vulnerable to your attacks. Use this to your advantage to strategically play and place defenses along this path to protect the castle.

<div><a class="image main"><img src="{{ "/images/The_Game_Board.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Setup Phase (Wave 0)
The game always starts in the Setup Phase (Wave 0) and will only start Wave 1 if the `Start next wave` button is clicked. Until then, you have time to set up towers and traps to stop the attackers in the coming waves. However, you cannot play spells until the wave starts. How to play each type of defense will be explained in more detail in the upcoming sections. Use this setup time wisely and prepare for the first wave. If you are ready, start the first wave.

### Enemies
The enemies are modelled as simple spheres. There are many types of enemy and each of them has different properties: speed, HP, damage, and even fly or not. They can be distinguished by different colors. Some of them are very strong, but don't worry, you will not face them in the early waves.

### Tower Cards
In order to build towers on the board, players have to place the **Tower** card within the camera field and on the game board. Towers can only be built on the game board. When placed correctly, two buttons will appear over the card: `Build Tower` and `Build Trap`. In addition to the two buttons, a range indicator will also be displayed over the card. It has the same appearance as a tower and the sphere around it demonstrates the attacking range of towers. So you can place your tower according to it.

<div><a class="image main"><img src="{{ "/images/Build_Menu.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

Click on `Build Tower` and select the type of tower that you want to build in the menu that shows up. Then click on one type of the towers to build it. Moreover, you cannot build one tower above another, but their ranges can overlap. Towers that the player cannot afford aren't available and are grayed out. During this building process the game is paused. The question counter will increase and you will be able to press the new button in the center to answer the question necessary to build the tower (see the *Answering Questions* section).

<div><a class="image main"><img src="{{ "/images/Build_Tower_Menu.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

 If the player correctly answered the question, the tower will be built and immediately start attacking enemies in its range. The image below shows an attacking archer tower and its arrow. For information on individual tower effects, check the in-game *Gallery*. You can again click on a tower to upgrade them. The detailed upgrade of all properties are shown in an upgrade panel, and you also need to answer questions to upgrade it with some costs.

<div><a class="image main"><img src="{{ "/images/Attacking_Tower.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Trap Cards
In order to build traps on the board, players have to place the **Tower** card within the camera field and on the game board. Traps can only be built on the game board. When placed correctly, two buttons will appear over the card: `Build Tower` and `Build Trap`. Click on `Build Trap` and select the kind of trap that you want to build in the menu that now opened. Traps that the player cannot afford aren't available and are grayed out. During this building process the game is paused. The question counter will increase and you will be able to press the new button in the center to answer the question necessary to build the trap (see the *Answering Questions* section). 

<div><a class="image main"><img src="{{ "/images/Build_Trap.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

If the player correctly answered the question, the trap will be built and immediately effect enemies walking over it. The image below shows a hole which slows down the enemies. For information on individual trap effects, check the in-game *Gallery*.

<div><a class="image main"><img src="{{ "/images/Hole.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Spell Cards
In order to cast spells, players have to place one of the twelve different ***Spell*** cards within the camera field and on the game board. Spells can only be casted when a wave is ongoing. The spell cards have the same appearance as in the *Gallery* but in dark blue. When playing a spell, you pay costs and draw a spell card from the spell desk, which contains a certain number of each spell. You can refill the spell deck with a certain cost manually by clicking the `Refill Spell Deck` button introduced in section *Game UI* at any time to compelement available spells. In order to make the best use of your currency, you are encouraged to cast all spell types properly. Of course, if you are confident with your strategy, you can also only use a few types of spells and directly refill the spell deck after they ran out. But the spells that you didn't use will not be added to the deck. 

When the camera recognizes the card on board, its icon will be displayed on the corresponding place together with the information `Draw <Spell Name> (In Deck: X) Cost: Y`, where X is the remaining cards of this spell in the spell deck, Y is the cost of this spell. If there is no this spell in the deck or the currency is not enough, `No <Spell Name> In Deck` or `Currency Not Enough, Cost: Y` would be displayed instead, respectively. 

<div><a class="image main"><img src="{{ "/images/Draw_Spell.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

By clicking on the spell image you can draw one spell card after successfully answering one question. Then, the information `Play <Spell Name> (In Deck: X)` will be displayed. You need to click the image again to play the spell. For spells that have a effect range, a sphere will be displayed as for the towers.

<div><a class="image main"><img src="{{ "/images/Play_Spell.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

Different spells have different effects and also visual effects. For spells that are effective during a period, there are also a ring-formed indicator to show the remaining time. Some spells also have collaboration between another. For example, thunder strike does more damage when it is raining. Play the game and try them out!

<div><a class="image main"><img src="{{ "/images/Meteor.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

### Answering Questions
The answering of questions will always be prompted when you want to play a spell, tower or trap card. If so, the question counter which located on the top of the screen will increase by 1 (for some cases may be more than 1) and you will be able to press the `View Qustion` button in the center to answer the question. A random question from the selected quiz will then appear and takes the whole screen space. Questions can either be multiple-choice (MC) or input questions. They can either with an image or not. Read the question description carefully. For MC questions, you need to choose one correct answer from at most five choices and then click `Enter` to submit. If you accidentally selected a wrong answer, pressing the answer again will unselect it. For input questions, you need to give the correct answer to the input field. Afterwards, also press `Enter` to submit it. If your answer is correct, the respective effect of the card is resolved as described in the above sections. If not, the card needs to be played again and you need to answer another question. In this case, the correct answer will also be given. When you are answering questions, the game is paused, so don't worry, you have enough time. Examples of different question types are illustrated below.

<div><a class="image main"><img src="{{ "/images/Question_Types.png" | prepend: site.baseurl }}" alt="" style="max-width: 100%;"/></a></div>

