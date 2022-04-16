# cosplaychessboard
HTML interactive chessboard for use when presenting a roleplay chess match onstage
Written by Alison Bird, Andrey Zholudok

## Table of Contents

1. Overview
2. Files
3. Configuration
4. User Guide

## Overview
### Background
Cosplay Chess is a live-action roleplay performance where persons dress as characters and act as chess pieces on a board. The game is acted on stage in real-time with music and other visual components. 
The Cosplay Chess Board Program is designed to display the current state of the board to the audience and provide background visuals during the fights that occur when a piece is taken. 


### Copyright
This program leverages a Javascript class called konva.js to render the board in HTML5. Below is the copyright license associated with said library. 

    /*
     * Konva JavaScript Framework v1.7.6
     * http://konvajs.github.io/
     * Licensed under the MIT or GPL Version 2 licenses.
     * Date: Wed Nov 01 2017
     *
     * Original work Copyright (C) 2011 - 2013 by Eric Rowell (KineticJS)
     * Modified work Copyright (C) 2014 - 2017 by Anton Lavrenov (Konva)
     *
     * @license
     * Permission is hereby granted, free of charge, to any person obtaining a copy
     * of this software and associated documentation files (the "Software"), to deal
     * in the Software without restriction, including without limitation the rights
     * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     * copies of the Software, and to permit persons to whom the Software is
     * furnished to do so, subject to the following conditions:
     *
     * The above copyright notice and this permission notice shall be included in
     * all copies or substantial portions of the Software.
     *
     * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
     * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
     * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
     * THE SOFTWARE.
     */

## Files
* CosplayChessboard.html - The main chess program. Contains all program logic. 
* background.png (1920x1080) - shown behind the chessboard during the match. 
* fightbackground.png (1920x1080) - shown when two pieces are called out for fighting
* attackvideo.mp4 (at least 2 min) - triggered during a fight for one video-based super attack
* participants (300x300) - pictures of the characters

## Configuration

1. Confirm with the Chess coordinator which team is on stage left (first) and stage right (second). There is an orientation variable that can be set to "left" or "right" to position A1. Default is left. 

2. Design a background and fighting background. Simply copy-paste the images into the directory and rename to background.png or fightbackground.png as needed. 

3. If there is going to a special attack video, copy-paste the MP4 video into the directory and rename to attackvideo.mp4. Any additional videos need to be played by Tech Ops in the room. 

4. Collect images of all the participants. 300x300 or 400x400 work best. 
Follow the naming convention for the pieces: 

			TEAM 1 (STAGE LEFT, ENTERS FIRST)
			piece 1 = top rook
			piece 2 = top knight
			piece 3 = top bishop
			piece 4 = QUEEN
			piece 5 = KING (ENTERS LAST)
			piece 6 = bottom bishop
			piece 7 = bottom knight
			piece 8 = bottom rook
			piece 9 = pawn
			piece 10 = pawn
			piece 11 = pawn
			piece 12 = pawn
			piece 13 = pawn
			piece 14 = pawn
			piece 15 = pawn
			piece 16 = pawn

			TEAM 2 (STAGE RIGHT, ENTERS SECOND)
			piece 17 = pawn
			piece 18 = pawn
			piece 19 = pawn
			piece 20 = pawn
			piece 21 = pawn
			piece 22 = pawn
			piece 23 = pawn
			piece 24 = pawn
			piece 25 = top rook
			piece 26 = top knight
			piece 27 = top bishop
			piece 28 = QUEEN
			piece 29 = KING (ENTERS LAST)
			piece 30 = bottom bishop
			piece 31 = bottom knight
			piece 32 = bottom rook
			
## User Guide
### Setup
1. Open the HTML in Chrome.  Hit F11 to expand to full screen. Hit CTRL+F5 to redraw the program
2. As pieces are announced, click on the squares they stand on. They can be clicked in any order. 
3. If the coordinator uses a PowerPoint to introduce pieces, pre-click all the pieces in full screen before kicking off the PowerPoint. 
4. Make sure the AV technical operations team cuts the feed to the center screen before switching from PowerPoint to the Chessboard
	
### Standard Actions
* To select a piece: click the piece once. A green boarder will appear around the selected piece.  To de-select, single click a selected piece. The green boarder will disappear. 
* To move a piece: Select a piece and then click on a new square. 

### Attack Actions
To attack a piece: select the attacking piece and click on the piece being attacked. 
This will trigger: 
1. Both pieces will be sent to the "Fight Screen". 
2. Click anywhere on the Fight Screen to return to the chess board. 
3. The attacking piece will automatically replace the attacked piece on the board. 
4. The attacked piece will be sent to their assigned space in the graveyard. 

To use the **special video attack**,  set up a standard attack. Then: 
1. Click on the gold star in the middle of the screen
2. This will launch a modular window with the video
3. To exit the video, click the "X" in the top right corner

### Swapping Actions
If you click any two pieces on screen that are on the same team, they will swap places, regardless of whether they are on the board or in the graveyard. 
This can be used for the following moves: 

**Castle:** Select the piece moving and click on a piece that is on the same team. The two pieces will swap places. 

**Pawn Upgrade:** click on the pawn on the board and click on the piece in the graveyard that they are being upgraded to (i.e. queen). 
* Pawn will be sent to the graveyard
* Upgraded piece will return to the board
	
**NOTE**: Any piece can also be returned to the board WITHOUT a swap. Click the piece in the graveyard and click any empty space on the board. 

### Game Pause
To put the entire screen into shadow and display "Cosplay Chess" across the middle: 
1. Click anywhere on the background to enact the Cosplay Chess shadow (e.g. for pauses, beginning, or end)
2. Click anywhere on the shadow to return to the main board
