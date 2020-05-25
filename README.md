# Elo
A simple Elo rating calculator

https://en.wikipedia.org/wiki/Elo_rating_system

## Dependencies:
python3

## Installation and Usage:

```
git clone https://github.com/Doekeb/Elo
cd Elo
./elo test.csv
```

Replace `test.csv` with a CSV file containing match results.
The CSV file should have two columns.
Each row represents a match where the first entry is the name of the winner and the second entry is the name of the loser.
Names should be unique and can include spaces.

```
usage: elo [-h] [-s] [-d] file [file ...]

elo is an implementation of the Elo rating system for zero-sum games.
https://en.wikipedia.org/wiki/Elo_rating_system

positional arguments:
  file                One or more CSV files, each representing a separate league. Each
                      row represents a single match, with the winner in the first column
                      and the loser in the second column. Entries in other columns will
                      be ignored and may therefore contain comments.

optional arguments:
  -h, --help          show this help message and exit
  -s, --show_history  Show all ratings updates.
  -d, --dynamic       Use dynamic (instead of static) k-factors.
```
