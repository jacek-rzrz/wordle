# Jacek’s Wordle Heuristics

Quick analysis of Wordle’s dictionary to find out what are good words to
start with and quickly hit as many target word characters as possible.

## Character distribution

There are 12974 words in the dictionary. This table shows how many words
contain each letter:

| char | n_words |
|:-----|--------:|
| S    |    5936 |
| E    |    5705 |
| A    |    5332 |
| O    |    3912 |
| R    |    3911 |
| I    |    3589 |
| L    |    3114 |
| T    |    3033 |
| N    |    2789 |
| U    |    2437 |
| D    |    2298 |
| Y    |    2031 |
| C    |    1920 |
| P    |    1885 |
| M    |    1868 |
| H    |    1708 |
| G    |    1543 |
| B    |    1519 |
| K    |    1445 |
| W    |    1028 |
| F    |     990 |
| V    |     674 |
| Z    |     391 |
| J    |     289 |
| X    |     287 |
| Q    |     112 |

Word count by character

## First guess

Characters **S, E, A, O, R** are the most frequent ones. They are all
contained by each one of these words:

AEROS, AROSE, SOARE

With any of the above words as the first guess, there is a 96% chance
that at least a single character from the day’s word will be hit, 69%
chance for unveiling two characters, and 24% chance for hitting as many
as three.

## Second guess

Characters **I, L, T, N, U** come as the next group in terms of
frequency. It’s possible to form a 5-character word from all of them
too:

UNLIT, UNTIL
