# Go Fish Card game using Python
Rules of Play
Initial Setup:
5 cards are distributed to two players (human player and computer).

The remaining cards form the central deck.

Gameplay:
The player starts by asking for a card. If the computer has the requested card(s), they are given to the player, and the player gets another turn.

If the computer does not have the card, it says "Go Fish," and the player draws a card from the central deck.

If the drawn card matches the requested card, the player gets another turn; otherwise, it’s the computer’s turn.

The computer follows the same rules, always asking for the topmost card in its stack.

Sets and Points:
A set is made when a player or the computer collects four cards of the same rank.

Points are awarded for each set made.

End of Game:
The game ends when either the player's hand, the computer's hand, or the central deck is empty.

The player with the most points wins.

Functions Used in the Code
init(self, cards=5): Sets up the game by creating and shuffling the deck, and distributing cards to the players.

validate(self): Checks if there are any sets in the player's hand and adds points accordingly.

go_fish(self): Returns the topmost card from the central deck.

core_mechanics(self, isPlayer, card): Implements the main game mechanics.

player_turn(self): Handles the player's turn.

computer_turn(self, isPlayer=False): Handles the computer's turn.

end(self): Checks if the game should end.

start(self): Starts the game.
