Flow

# Menu options
## Config
Configure

## Search
Search  -notes 
        -phrases
        -pieces
        -sessions
        -plays
        -gigs

## Create
Design  -note
        -phrase
        -piece
        -session
        -variation
Play a session
Reflect on a gig

## Generate
Generate a session

# Configuration options
## Note option lists. Those appear as choices when designing notes.
Dynamics
Articulation
Instrument
Limb
Grace Note

## Available options per instrument as above including default, can also add an option on the fly and it will be added to the 
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
## Note

Upon filling an option, if it conflicts show the conflict next to the options. If articulation is rim, but chosen HH for example.
Upon save check whether a duplicate exists and ask to change name/representation
Duplicate is same dynamics/articulation/instrument/limb/grace-note
Clash name? Ask to change this one or the other one.

<CR> to move to next option
<Arrow Down and Up> to move around
<Arrow Left and Right> to choose options, or move within text field
<Tab> <Shift-Tab> to move around
<Backspace> and <Delete> do their thing

----- Design a note -----

Name:           _____ [free text. string]
Dynamics:       _  [p/f/_]
Articulation:   _____ [one of options. prefilled based on instrument/limb]
Instrument:     __ [one of options. prefilled based on articulation/limb]
Limb:           _ [R/L/K/H. prefilled based on instrument]
Grace note:     ____ [flam/drag/_]
Representation: _ [single character]
Remarks:        _____ [free text. string]

SAVE/CANCEL

-----<------------->-----

## Phrase

Count and Subdivision both prefilled to 4
Changing Count adds/removes counts [warning about deleting notes]
Changing Sudivision add/removes columns and changes counting [warning about deleting notes]
When moving highlight line and column
Add a way to override representation on demand
Be able to load a phrase from search as a starting point

----- Design a phrase -----

Name:         _____
Display name: _____
Count:        _
Subdivision:  _
CLEAR [when things get messed up]
--------------------------

    1 e & a 2 e & a 3 e & a 4 e & a
SD  O   o   O   o   _ [_ -> R    drum        -> _                  ] Press <CR> at any point to place with defaults
__                    [p    L -> rimshot        flam -> place note ]
                      [f         cross-stick    drag               ]
                        

-------------------------
Remarks: _____


## Piece
The preview can be toggled off/only for selected section/any selected sections/all
You can create a new section if you need
Song, artist, etc. metadata suggestions come up as you're typing, <CR> confirms the autosuggestion, <ESC> cancels autosuggestion until next keypress, 
You can drop in a section and modify it on the fly and save it with a different name

----- Design a piece -----

Name:  _____   Song:    _____
Tempo: ___     Artist:  _____
Feel:  _____   Drummer: _____
               Album:   _____
               Year:    ____

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


## Play
Be able to edit the pattern on the fly and save it as a different one
Start and stop the timer with a button. Restart possible until save.
Ask for date when beginning session and fill it in for all plays

----- Play -----
Date:     __/__/__
Start:    __:__
End  :    __:__
Duration: __:__

Tempo:  ___
Rating: _

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


## Session
Be able to use a previous session as base
Dont have to give a date
Number automatic
Plays are chosen from a list of phrases, and wrapped in a play


----- Design a Session -----
Number:  _____
Date:    __/__/__
Remarks: _____

1. Warm-up 1
2. Doubles
3. ______
