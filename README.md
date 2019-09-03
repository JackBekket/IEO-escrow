# IEO-escrow
Escrow contracts for exchange listing / IEO


Lately, we could see a lot offerings about IEO / exchange listing

How we can get a protection from *scum* offering? 

I suppose we could use simple escrow contracts, which could provide safe escrow deals for listing.


Basic mechanic is:
1. escrow mechanism based on https://github.com/JackBekket/escrow-eth
2. deal start with locking funds from buyer, with storing address of 'seller of exchange offering' + address of exchange
3. after some freeze period, contract ask address of exhcange about `balanceOf()` of some token
4. if it exist - funds go to the seller, if not - return to the buyer

Any advices are welkomed in issues.
