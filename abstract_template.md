


Abstract cards:

required operations + time expectation
optional operations + time expectation
Above possibly notated by a list of all possible operations, with one edge-printed color for required and another for optional, and all other operations listed but greyed out and neutrally labeled. Time expectation might turn out to always be consistent per-operation, rather than per-card, in which case it could be denoted elsewhere -- for example, an info sheet providing an explanation of the operations.

Each abstract card could have "notches" of some type that allow you scan the list of concrete cards to find any that fulfill its required operations by looking at the edge-printed colors on the stack of concrete cards. Or this could be something we instruct people on doing, if they're only going to use them as reference cards and not for gameplay.





A list of all the abstract data structures. Possibly some general notes on them too, but note that the card details section contains notes pertaining specifically to abstract data structure cards as well. Note also that each card should have its own page, and this will just link to all of them.

STACK

push: add to end pop: remove from end

*peek: get value of next pop *count: get length

implementations: :: linked list: O(1) :: array: O(1), but fixed size [you can only have one at a time], mutation? :: dynamic array: O(1), amortized, (mutation?)

--> historical note: Turing was the first one to refer to a stack, called operations 'bury' and 'unberry' --> sigs from Turing's grand-students

QUEUE

enqueue: add to end dequeue: remove from other end

*peek: get value of next dequeue *count: get length

implementations: :: doubly linked list: O(1), mutation :: linked list w/ tail pointer (add to tail): mutation :: array: O(1) if you treat it like a ring buffer, mutation, fixed size :: dynamic array: amortized O(1), mutation :: banker's queue: O(1), amortized, [persistent with more work], [non-amortized with more work] -> Tarjan: persistent -> Okasaki: amortized

--> history?

DEQUE

push: add to end pop: remove from end shift: add to front unshift: remove from front peek-last: get value of end peek-first: get value of front

*count: get length

implementations: :: doubly linked list: O(1), mutation :: array: O(1) if you treat it like a ring buffer, mutation, fixed size :: fully persistent is tricky, catenable [], confluently persistent [mergable, like github, makes a DAG], else ephemeral. partially persistent is read-only.
