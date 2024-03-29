# Hearts
AIClass Structure
Value enum
Suit enum
Card class (for each individual card)
Deck class (for the "deck" to deal hands)
Hand class (for each of the hands)
Player abstract class (defines base functionality for any player)
HumanPlayer class extends Player (performAction() allows human input)
State class (track state of the game and allow for random playouts)
Game class (plays one game)
Hearts class (this is the main file that brings it all together)
Implemented Players
HumanPlayer: Allows humans to play Hearts
LowPlayAI: Picks the lowest card in a valid suit
RandomPlayAI: Plays a random card in a valid suit
LookAheadPlayer: Looks ahead a minimal amount of steps to make a decision
MCTSPlayer: Uses MCTS to decide on the optimal next move
Version History
0.0.1 — Setting all of the infrastructure up and testing some java things
0.0.2 — Implemented abstract player as well as basic human player skeleton
0.0.3 — Begun implementation for game playouts
0.0.4 — Able to do multiple playouts of the game
0.0.5 — Able to keep track of cards played for each round
0.0.6 — Game keeps track of the scores of each player now!
0.0.7 — Game keeps track of scores between games; games do initialization properly now
0.0.8 — HumanPlayer can now select which card to play, with Exception Handling!
0.0.9 — Added card "shorthand" display using unicode characters (and reordered suits)
0.0.10 — Game now checks if the played card by the Player is valid! (for ALL cases)
0.0.11 — Game now checks who the "winner" of each round is!
0.1.0 — First full game implemented! (With no state tracking functionality for AI)
0.2.0 — Game now passes in currentRound to performAction()
0.3.0 — Working Low-Play AI has been completed
0.4.0 — Added score-tracking statistics
0.5.0 — Shooting the moon is implemented — minor bug fixes as well
0.6.0 — Added a copy constructor for the Deck and began working on the State class
0.6.1 — All Players now take parameters of the State class, State constructor now finished
0.6.2 — Added functionality to return the range of cards in any given suit
0.6.3 — RandomPlayAI has been implemented completely and is working
0.6.4 — MCTSPlayer implementation has begun
0.6.5 — LookAheadPlayer implementation has begun
0.7.0 — Implementation for advance() within the State class has begun
0.7.1 — advance() now checks for validity of the selected move
0.7.2 — Design paradigm for multiple game playouts has been established
0.8.0 — Finished preliminary version of advance() in the State class
0.8.1 — Added functionality for displaying debug messages only for Human players
0.8.2 — Fixed printout issue with shooting the moon — random AI able to shoot the moon!
0.9.0 — LookAheadPlayer has performAction() implemented (but not playoutGame())
0.9.1 — Fixed shallow copy issues with Decks and hands
0.9.2 — Playthroughs with state and lookahead player both work! Fixed minor issues
1.0.0 — Full working game, with working State class, game playthroughs, and LookAhead AI
1.0.1 — Finished skeleton of MCTS Player
1.0.2 — Fixed bug with advance() method in the State class with returning accrued points
1.0.3 — Most MCTS functions have been written; just need to deal with random playouts
1.0.4 — Debugging process for MCTS — fixed an issue with treePolicy()
1.0.5 — All MCTS functions except assignReward() now are fully functional
1.0.6 — Preliminary completion of assignReward() function
1.0.7 — MCTS completed and running — checking for validity of results now
1.1.0 — MCTS player completed (but not optimized) for now

Future Work
Decouple Hand and Player operations by creating a new Hand class
Fix how cards are removed from the hand/selected by Players
