Name of Structure
=================

## Feature list [bold RHS if applicable]
- mutation / immutable [if *any* operations are implemented with mutation (even benign effects)]
- ephemeral / persistent
- not / fully persistent
- not / confluently persistent
- not / catenable
- amortized / worst-case [if *any* operations are amortized]
- fixed / growable
- jumbled / ordered [how do we designate insertion order vs sorted vs etc?]


## Operation list / performance characteristics
- push-fast: 
- pop-fast: 
- peek-first: 
- push-slow: 
- pop-slow: 
- peek-last: 
- length: 
- lookup (nth element or by key): 
- insert (in middle or by key): 
- update (in middle or by key): 
- memberof: 
- slice: 
- max element (or min): 
- nth greatest element: 
- merge (only for catenable? or is that feature only for functional?): 

## Other performance factors
E.g., wasted space, other spatial concerns, best/average/worst case divergence (some kind of std dev or Q factor, maybe), unusually large constant factors, locality concerns, parallelism concerns, GC implications, etc.

## Historical tidbit / interesting quote / etc

## Signatures and associated power-ups, if applicable


-------------

Notes:

Ops colored by green / yellow / red / black (or some such):
- GOOD (green): fulfills this as quickly as possible, no real downsides (bounded amortization is okay)
- OKAY (yellow): off from max by factor of O(log n), or poor spacial characteristics, or unbounded amortization, etc. (note that O(log n) time *plus* O(log n) extra space is SLOW)
- SLOW (red): off by factor of O(n) time, or other equally bad properties (note that O(n) time *plus* O(log n) extra space is DIRE)
- DIRE (black): can not reasonably achieve the operation
The colors should be edge-printed so it's possible to quickly scan the deck to find good performing data structures for a particular set of operations.

It could be that sigs unlock extra ops (ones that aren't usually included in that implementation, e.g. because they raise the constant costs), and those are colored pink or something to indicate that they're outside the usual spectrum but can still apply. For example, you could store a pointer to the tail of a linked list, hence giving O(1) peek-last (but nothing else). If there are common optimizations applied to the basic data structure this is a good place for them.

If ops require extra space put the spacial complexity in. If we know the actual constants use tight bounds instead of asymptotic complexity (or mix them, Knuth-style). If we know the amortization bounds put those in (or just 'amortized' if it's unbounded) [this might be very implementation dependent, in a way that we don't want to track... maybe just knowing that it's boundable is enough. (Is it always boundable?)]. 

Each card has a unique url on the DSC site that provides more detailed information, algorithms, links to papers and resources, quotes, etc.

Each concrete card also has both a data structure diagram and a whimsical representation.