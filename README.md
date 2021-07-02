# 3-card-poker
I made this program over a year ago while I was bored on a train ride. I'll start by explaining the game of 3 card poker:  3 Card Poker is played with a 52 card deck and at least 2 players (one being the dealer), and a maximum of 3 players. The object of the game is similar to blackjack in that it is "against the house". The round begins by each player placing a bet of whatever amount they choose. The dealer then deals 3 cards face up to each player, and then 3 cards face down in front of themself. Each player has the option after looking at their cards to fold, or place the same bet they placed at the start again to continue the round. This is where my program is intended to come in handy, as it can give the player a better guess of whether they should fold or double down and stay in. After all players have chosen to fold or play, the dealer flips their cards. If any player has a better hand than the dealer, they double the total amount they put in. This isn't actually true in all cases though, let me explain:  The way that the house sways the odds of this in their favor is by having the dealer "not play" any hand worse than a queen high. Let's use an example. I bet $50,000, and am then dealt 3 aces of different suits. Obviously, I am going to go in with that hand - forcing me to double my bet to $100,000 total. The dealer then flips their cards to reveal an off suit 3, 8, and jack. Because the dealer didn't "play", as they has a worse hand than a queen high, I only win an additional $50,000 on this hand instead of the full $100,000 being doubled. This means that it is impossible to win a hand if you have less than a queen high, and the best that you could get is the dealer not playing the hand. You can test this with the code, as if you input any hand below a queen high you will see your win percentage is 0, so it is often not worth entering the round and you must stomach losing your initial bet. On to the discription of the program:     I created a program with an intermediate Python GUI made with Pygame, that calculates the odds of any given hand of 3 card poker. The program works in the following stages:  -Graphically prompts the user to give the number of players at the table with a face-up hand .  -Shows a screen with every possible card in a deck, and the user clicks their 3 cards that are held in their hand.   -Program calculates the percentage of possible cases in which the given hand wins, loses, or the dealer doesn't play. It then converts them to a percentage of the total possible hands, and displays them on screen with an option to restart and enter a new hand.  There are obviously many interim steps to improve the programs functionality and visual design, but those are the 3 primary steps.