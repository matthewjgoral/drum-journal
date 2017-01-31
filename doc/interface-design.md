Flow

# Menu options

## Search
Search
- phrases
- pieces
- sessions
- performance
- gigs

## Create
Design
- phrase
- piece
- session
- variation
Play a session
Reflect on a gig


## Generate
Generate a session

## Config
Configure

# Configuration options
## Note option lists. Those appear as choices when designing notes.
Dynamics
Articulation
Instrument
Limb
Grace Note

## Available options per instrument as above including default
can also add an option on the fly and it will be added to the list above

SD Dynamics -all -_
   Articulation #{drum, rimshot, cross-stick} -drum
   Limb #{R, L} -R
   Grace
HH
...

## Sudivision options
Counting 1
         2 &
         3 t l
         4 e & a
         5  
         6 t l & t l

# Design interface

## Phrase

Count and Subdivision both prefilled to 4
Changing Count adds/removes counts [warning about deleting notes]
Changing Sudivision add/removes columns and changes counting [warning about deleting notes]
When moving highlight line and column
Add a way to override representation on demand
Be able to load a phrase from search as a starting point
Place previous note shortcut
Place previous note and open menu shortcut
Repeat previous beat
Move selected notes up/down
Increase/decrease dynamics
Add flam/drag
Change articulation - change display

~~~~~
----- Design a phrase -----

Name:         -----
Display name: -----
Count:        -
Subdivision:  -
CLEAR [when things get messed up]
---------------------------

    1 e & a 2 e & a 3 e & a 4 e & a
SD  O   o   O   o   _ [_ -> R    drum        -> _                  ] Press <CR> at any point to place with defaults
--                    [p    L -> rimshot        flam -> place note ]
                      [f         cross-stick    drag               ]
                        

--------------------------
Remarks: -----
~~~~~


## Piece
The preview can be toggled off/only for selected section/any selected sections/all
You can create a new section if you need
Song, artist, etc. metadata suggestions come up as you're typing, <CR> confirms the autosuggestion, <ESC> cancels autosuggestion until next keypress, 
You can drop in a section and modify it on the fly and save it with a different name - Default name: Song-section-[give name]-1

~~~~~
----- Design a piece -----

Name:  -----   Song:    -----
Tempo: ---     Artist:  -----
Feel:  -----   Drummer: -----
               Album:   -----
               Year:    ----

Remarks:
--------------------------

| INTRO | VERSE1 | CHORUS | ____ |
|-------|--------|--------|------|
|   4   |   8    |   8    |      |
|-------|--------|--------|------|
| "note"| "bla"  | "bla"  |      |
|-------|--------|--------|------|
            |
            v [Preview opens]

    1 e & a 2 e & a 3 e & a 4 e & a 1 e & a 2 e & a 3 e & a 4 e & a 
HH  x   o   x   x   x   o   x   x   x   o   x   x   x   o   x   x   |
HT  |       :       :       :       |       :       :       :       |
SD  |       O     o :       :   O   | o     O       :       O       |
LT  |       :       :       :       |       :       :       :       |
BD  O       :       O   O   :       |   O   :       O   O   :       |
HF  |       x       :       x       |       x       :       x       |
~~~~~

## Session
Be able to use a previous session as base
Dont have to give a date, but can if you want to plan ahead. Will be changed to whenever you actually performed it.
Number automatic (yearmmddhhmm of start of performance)
Plays are chosen from a list of phrases, and wrapped in a play

~~~~~
----- Design a Session -----
Number:  _____
Date:    __/__/__
Remarks: _____

1. Warm-up 1
2. Doubles
3. ______
~~~~~

# Perform interface

## Start a session
Resume session (if on a different day ask if append or save as a new session, if on same day just append)
Start a new session
    Choose a saved session
    Create a new session based on previous
    Create a new session from scratch

## Run a session
Date autofilled
Choose each section
Shortcuts for open next session
Put in a new performance (choose phrase, section, piece and make new/existing/modify existing)
Alter time

~~~~~
Date:     __/__/__

[05:12] Warm-up 1 
[--:--] Doubles
[--:--] Bass drum skank practice
...

PAUSE
END
~~~~~

## Play something

Be able to edit the pattern on the fly and save it as a different one
Start and stop the timer with a button. Restart possible until save.
Ask for date when beginning session and fill it in for all plays
Start/pause clock [CR?]
Pop up to selection list and pause/pop back and manually resume
Stop and record

~~~~~
----- Play -----
Duration: __:__ (in seconds)

Tempo:  ___

    1 e & a 2 e & a 3 e & a 4 e & a 1 e & a 2 e & a 3 e & a 4 e & a 
HH  x   o   x   x   x   o   x   x   x   o   x   x   x   o   x   x   |
HT  |       :       :       :       |       :       :       :       |
SD  |       O     o :       :   O   | o     O       :       O       |
LT  |       :       :       :       |       :       :       :       |
BD  O       :       O   O   :       |   O   :       O   O   :       |
HF  |       x       :       x       |       x       :       x       |

________________
16/01/16 -- 100 -- G -- 10:12
[other dates and details of practice]
~~~~~


# Search interface

## Search phrases

~~~~~
----- Search phrases -----
CLEAR

Name:         -----
Display name: -----
Count:        -
Subdivision:  -
Remarks:      ____
---------------------------

    1 e & a 2 e & a 3 e & a 4 e & a 1 e & a 2 e & a 3 e & a 4 e & a 
HH  |                               |                               |
SD  |       O     o :       :   O   | o     O       :       O       |
BD  O       :       O   O   :       |   O   :       O   O   :       |
HF  |       x       :       x       |       x       :       x       |


~~~~~


