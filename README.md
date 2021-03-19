# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Johnny Ong

Time spent: **2.5** hours spent in total

Link to project: (https://glitch.com/edit/#!/quickest-road-stage)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![](http://g.recordit.co/opd2qNynDe.gif)
![](http://g.recordit.co/60vKXYHyuM.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random
https://www.w3schools.com/cssref/css_colors.asp

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

An issue I encountered was the playClueSequence function as the function didn't run when I hit "Start". To fix this, I first looked at the console output
in my browser's Developer Tools. In there, I saw that an error was displayed that was pointing to my  lightButton()/clearButton() functions. Apparently,
I had made a typo and instead of classList I accidently put checkList. A smaller issue I ran into was when I playtested my game. The game ran smoothly
for the first three iterations but failed on the fourth iteration. To be more specific, the pattern played correctly but when I did my "guess" which was
correct, the game deemed it incorrect. The issue was that my guessCounter wasn't being set to 0 after each round because I had a typo making it guesscounter.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

The implementation of this game was easy enough, so what would the implementation of a Flash/Unity game would look like? 
 - I know that those types of games are created in the Unity engine so I would assume that some APIs are involved to link the game and display it to the user.
How does having different tabs work?
 - This game was all made in one web browser tab so I didn't have any practice or even know how to create and navigate through different parts of a website]
In the application, there were several different technologies listed, would using those technologies have made the implementation of this game easier?
  - As a follow up, what do those technologies do? I know that MongoDB is for databases and Heroku is for deployment, but I don't have much knowledge on the rest
How do I publish/deploy this game?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

The first thing I would do would be to look over the sound function/library more to understand it better then add in custom sounds. I feel that the
getting the sound is the most technically difficult part of this tutorial (although I did understand it well enough and had no issues) and had the most components while everything else was relatively easy. 
As such, I would want to play around with the library more to get a better feel. The second thing I would do is make the game more "Simon Says" looking. 
In the physical version of Simon Says, the game is a circle with each color being a quarter of a circle. Thus, I would want to make this web version look
similar to the real life version for some authenticity as well as learning a bit more about html/css.



## License

    Copyright Johnny Ong

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
