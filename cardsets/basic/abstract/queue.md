QUEUE

enqueue: add to end dequeue: remove from other end

*peek: get value of next dequeue *count: get length

implementations: :: doubly linked list: O(1), mutation :: linked list w/ tail pointer (add to tail): mutation :: array: O(1) if you treat it like a ring buffer, mutation, fixed size :: dynamic array: amortized O(1), mutation :: banker's queue: O(1), amortized, [persistent with more work], [non-amortized with more work] -> Tarjan: persistent -> Okasaki: amortized

--> history?




QUEUE

enqueue: add to end
dequeue: remove from other end

*peek:   get value of next dequeue
*count:  get length

implementations:
:: doubly linked list: O(1), mutation
:: linked list w/ tail pointer (add to tail): mutation
:: array: O(1) if you treat it like a ring buffer, mutation, fixed size
:: dynamic array: amortized O(1), mutation
:: banker's queue: O(1), amortized, [persistent with more work], [non-amortized with more work]
    -> Tarjan: persistent
    -> Okasaki: amortized

--> history?
