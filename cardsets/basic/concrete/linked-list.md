Linked List (Persistent)
=================

## Feature list [bold RHS if applicable]
- ephemeral / *persistent*
- not / *fully persistent*
- not / confluently persistent
- not / catenable
- amortized / *worst-case*
- mutation / *immutable*
- fixed / *growable*
- jumbled / *ordered* / sorted


## Operation list / performance characteristics 
- push ("fast" end): FAST O(1)
- pop: FAST O(1)
- peek-first: FAST O(1)
- shift (change these names; also these are from the "slow" side, whatever that is): 
- unshift: 
- peek-last: DIRE O(n)
- length: DIRE O(n)
- nth element (direct access): DIRE O(n)
- insert in middle: 
- max element (or min): 
- nth greatest element: 
- key/value lookup (hmmm. what about adding?): 
- merge (only for catenable? or is that feature only for functional?): 

## Other performance factors
- 50% wasted space

## Historical tidbit / interesting quote / etc

## Signatures, if applicable



-------------

Notes:

Ops colored by green / yellow / red / black:
- FAST (green): fulfills this as quickly as possible, no real downsides (bounded amortization is okay)
- SLOW (yellow): off from max by factor of O(log n), or poor spacial characteristics, or unbounded amortization, etc
- DIRE (red): off by factor of O(n), or other equally bad properties
- BLANK (black): can not reasonably achieve the operation

If ops require extra space put the spacial complexity in. If we know the actual constants use tight bounds instead of asymptotic complexity. If we know the amortization bounds put those in (or just 'amortized' if it's unbounded) [this might be very implementation dependent, in a way we don't want to track... maybe just knowing that it's boundable is enough. (Is it always boundable?)]. 


Four different levels of design:
- simple consistent card back
- accurate image for each DS (design language for representing structural aspects)
- overall layout for the card information (plus mod knobs for expansion decks)
- fancy image for each DS (should to be able to commission these widely)

Each card has a unique url on the DSC site that provides more detailed information, links to papers and resources, quotes, etc.