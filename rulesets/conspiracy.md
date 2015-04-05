Conspiracy: Hack the Mainframe.
===============================

A cooperative game for one to six players.

Cards: Any abstract and concrete cards, including any expansion deck cards. Including more abstract cards makes it harder. Including more concrete cards makes it easier.

Additional pieces required: 
- a timing device, preferably digital.
- coins or other homogeneous markers
- (dice, pencil/paper, spinners, chessboards, gemstones, etc)

###Story

There's a conspiracy attempting to keep you and your friends from learning about data structures. To overcome this vile plot you're going to have to... yep, you guessed it. You're going to have to hack the mainframe.

###Setup

Shuffle the  abstract cards and put them face down to one side of the table. This is the mainframe. If you manage to fulfill all the requirements for hacking in to it you all win. If you fail even one requirement you all lose.

Deal out N cards to each player. Put the remaining concrete cards face down on the opposite side from the abstract cards. [Turn the top M concrete cards face up. Players can swap out with these cards instead of taking their turn.]

###Gameplay

The goal of the game is to work your way through each layer of the mainframe's security. You'll need to work together to do this, because each of you only has a limited number of resources available for meeting the requirements for hacking a layer of security.

Choose a starting player [by some means, e.g. most colorful attire]. Gameplay proceeds to the left. For the first round, they flip the top abstract card of the mainframe. They then have a chance to try to fulfill the requirements on that card by using one of the cards they are holding. 

For example: 
The current security layer requires a queue. I have a [...] in my hand. If I play it against the queue I'll lose two turns, because of the SLOW behavior for pop-slow. So instead I'll play my [...] and only lose one turn because of [...]

Choose exactly one action each turn:
- fulfill the current security layer's requirement
- swap up to two cards with the M up-facing concrete cards.
- draw a concrete card (not more than N+K in hand at once)

Ending conditions:
- break the last security layer -- you win! woo!
- go an entire round without breaking the current security layer -- you lose :(
- (for one player games you may play up to L rounds)
- (for two/three player games, special rules apply... oh, maybe the number of cards varies? N-(#ofplayers)?)

###Rules for partial fulfillment

- an OKAY fulfill costs a turn
- a SLOW fulfill costs two turns
- a DIRE operation can't ever fulfill
- for special effects, consult the list (but generally lose one turn)

You can swap cards on your lost turns, but can not draw new cards or break through a security layer.

###Upon breaking a security layer

Each player keeps the security cards they have broken through. [The mainframe somehow marks them?] The following pros and cons apply, based on how many abstract cards you have collected:
1. 
2. 
3. 
4. Hard real-time: fulfillment with an [unbounded?] amortized card costs a turn, but [...]
5. Purely functional: fulfillment with a mutating card costs a turn, but a non-mutating card can fulfill multiple security layers, if there are multiples.
6. 
7. Fulfillment penalties are doubled, but you can swap three cards instead of two.
8+. Start a timer for 10 seconds before the security layer is revealed. If the timer goes off before the layer is broken you all lose. The player with eight cards may, after the abstract card is revealed, choose the player who will start the round (who will play next, and whose subsequent turn arriving without having broken the layer is a losing condition).

If two players have the same number of security cards, then on the next round two abstract cards are turned over. [They can be dealt with in either order.]. If three, then three cards, and so on.

[Maybe a system for passing a card to your right. It might take your turn to do so.]

Once a player breaks a security layer, it is the next player's responsibility to reveal the new one. [Is it only that player's pros/cons that take effect on the next round?]



Later:
maybe I need a queue for a hard real-time system. I look at the cards in my hand and try to find one that will fulfill those requirements. I've got a Banker's Queue, but it's amortized and kills my temporal guarantees. I could play it but I'd occasionally lose a turn for the rest of the game. 

I could play my trusty doubly-linked-list instead, and eat the cost of mutation and lack of persistence. There's a lot of binary attributes that concrete data structures either possess or don't, and a lot of ways of slicing up the performance characteristics for the operations they support. In a perfect world the cards and rules would be very simple, but learning to play the game would teach you actual valuable lessons you could apply in the programming world.
