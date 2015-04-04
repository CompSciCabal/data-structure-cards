Linked List (Persistent)
=================

## Feature list [bold applicable side]
- mutation / *immutable*
- ephemeral / *persistent*
- not / *fully persistent*
- *not* / confluently persistent
- *not* / catenable
- amortized / *worst-case*
- fixed / *growable*
- jumbled / *ordered*


## Operation list / performance characteristics 
- push-fast: FAST O(1)
- pop-fast: FAST O(1)
- peek-first: FAST O(1)
- push-slow: DIRE
- pop-slow: DIRE
- peek-last: SLOW O(n) time
- length: SLOW O(n)
- lookup (nth element or by key): SLOW O(n)
- insert (in middle or by key): DIRE
- update (in middle or by key): DIRE
- memberof: SLOW O(n)
- slice: SLOW O(n)
- max element (or min): SLOW O(n)
- nth greatest element: SLOW O(n)
- merge (only for catenable? or is that feature only for functional?): 

## Other performance factors
- 50% wasted space on pointers
- tail-sharing for compact full persistence

## Historical tidbit / interesting quote / etc

## Signatures, if applicable

