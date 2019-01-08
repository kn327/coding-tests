# Playing Cards

Challenge:
Write a program that models a deck of playing cards.

1. Construct a valid 52 card deck, with 4 suites and 13 cards (Ace through King) of each suit.
2. Shuffle the deck so that cards are randomly distributed (each run of the program should produce a different random distribution).
3. Deal a hand of five cards to five different players (build the hands by dealing one card from the deck to each hand, passing around the players 5 times).
4. Write the hands out to console with each hand sorted by value in ascending order (with Ace being the highest value)
5. Each card should be written out as value followed by suit:
    a. Values = 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K, A
    b. Suits = H, D, S, C (Heart, Diamond, Spade, Club)
6. Each card should be separated by a dash.
7. We are looking for object-oriented programming techniques: at a minimum you should have classes to represent a Card, Deck and Hand.

The resulting output should look like the following:\
Player #1: 2C-3H-5D-9H-AS\
Player #2: 5C-8S-10H-QS-KC\
Player #3: 3D-8C-8H-9C-AH\
Player #4: 6H-7C-KD-AD-AC\
Player #5: 4S-4C-9D-10C-10S
