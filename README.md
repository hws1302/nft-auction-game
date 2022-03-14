# Non-fungible Token (NFT) Auction Game

This is a part of the Crypto Trading Course by IMC and the first time I've looked at NFTs.



## What are NFTs?

NFTs are tokens on the blockchain which are unique cannot be created again (i.e. non-fungible). These tokens on the blockchain can be associated with art through websites such as [opensea.io](https://opensea.io/).

We were looking at the *Bored Ape Yacht Club* (BAYC) which is a collection 10000 NFTs. Apes have 6 characteristics (background colour, fur style, mouth style, eyes style and hat), which are shared e.g. over 500 apes have 'bloodshot' eyes, but no two apes have exactly the same combination of all characteristics. Some NFTs are more rare than others e.g. for BAYC golden fur is very rare. Rare characteristics strongly correlate with the price. 


## How the game works 

We were provided with a subset of the apes (~3300) in a CSV along with their characteristics and were given $300. An auction was then held where the apes would be given a score by rarity. If we met the following rules, our top 6 apes would be added up to give a final score:

- Apes bought must not exceed $300
- Must have one ape of each background colour 
- Must have one ape with solid gold fur

The score assigned to each ape was the sum of the inverse rarities for each trait (where the rarity is the number of instances of a charactersitic / total number of tokens), the that the score increases with the rarity.

To calculate the score for the ape in the photo below:

- Background: Yellow (17.00%)
- Fur: Solid Gold (0.052%)
- Clothes: Black T (4.10%)
- Mouth: Small Grin (2.54%)
- Eyes: Laser Eyes (0.70%)
- Hat: Sea Captain's Hat (5.32%)


1 /0.1700 + 1/ 0.0052 + 1 /0.0410 + 1/ 0.0254 + 1 /0.0070 + 1 /0.0532 ~ 429 

There is also a **wildcard** token which boosts the players final score by 20% but doesn't count as one of the six tokens. 


## What I've considered

- Atleast one token with solid gold fur how many players are there, get it early?
- How should token valuations change with time 
- Come up with way to check the incidence
- Which ones have the largest shift in rarity
- Backgrounds all have roughly the same occurance so this won't be an input into the model 
- How should the value of a background increase if you don't have it 
- Should you ever buy more than 6? 

![Image of Token](https://ipfs.io/ipfs/QmQpxqZ6hPnx8ofapPVgbg9JAh7S9oh3fNYvWwU7okdCU8)
