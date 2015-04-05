DEQUE

push: add to end pop: remove from end shift: add to front unshift: remove from front peek-last: get value of end peek-first: get value of front

*count: get length

implementations: :: doubly linked list: O(1), mutation :: array: O(1) if you treat it like a ring buffer, mutation, fixed size :: fully persistent is tricky, catenable [], confluently persistent [mergable, like github, makes a DAG], else ephemeral. partially persistent is read-only.




DEQUE

push: add to end
pop: remove from end
shift: add to front
unshift: remove from front
peek-last: get value of end
peek-first: get value of front

*count:  get length

implementations:
:: doubly linked list: O(1), mutation
:: array: O(1) if you treat it like a ring buffer, mutation, fixed size
:: fully persistent is *tricky*, catenable [], confluently persistent [mergable, like github, makes a DAG], else ephemeral. partially persistent is read-only. 

--> history?
