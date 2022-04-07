# Motivation

This game was designed with [Rarity Manifested](https://github.com/andrecronje/rarity) in mind.
Rarity was a great experience that tried to build on what the [Loot (for adventurers)](https://www.lootproject.com/) project started: a community owned, accessible and highly creative experience.

Loot's base system is simple: a set of 8000 NFTs, each representing a set of RPG items.
After that, it was up to participants to build the rest of the universe.
There was a token, fan made derivatives such as lands, adventurers, etc.
But this approach had a downside:

- The limited number of NFTs made it hard to get, reducing the size of the core community.
  Not everybody in a community is capable of building on a blockchain and the limited stock + high demand + high fees reduced prevented potential community involvement.
- As the project was oriented toward high creativity, a lot of initiatives pushed the project in many different directions without really achieving long lasting, sustainable efforts.

Rarity addressed this issue by moving to Fantom, making it free for anyone to create an adventurer and giving a direction to the project by following Dungeons & Dragons guidelines.
It worked very well, with Rarity becoming one of the most used contract on Fantom.
But there were also limiting factors:

- Using a better defined base system made the ecosystem dependent on changes of the base. Not all contracts were available at the start and you had to wait for them to be available before building. For example, several community members wanted to have a skill system before the "official" one came out but spending time doing it would have been useless as the rest of the community would have used the official one when it becomes available. In general, despite the fact that was autonomous, it was highly centralized around the base implementation.
- Lack of sustainable financing of developments. As everything in the project is free, contributions were only open source. While this is great while it lasts, economic incentives help sustain work. There was a grant program, but it was just "VC money" charitably given to builders.
- Lack of leadership. The creator of Rarity explicitly wanted the project to be community driven. However, as explained in the points above, there was still some degree of centralization due to the structure of the project. This adds friction for contribution, as builders have to either get integrated in the official repository or be integrated in one of the main web UIs to have a chance to exist.
- Excessive botting. The game is so accessible that it's basically free to manage an army of adventurers. In-game items are therefore mostly worthless, as they can easily be farmed to infinity. This is making it hard to build any real value in the game, once again preventing financial sustainability.

The solutions for these issues that **Sanctis** is proposing are the following:

- A fully modular base system that allows using templated components and only adding game logics to them. This gives builders a framework to enhance composability and interactions with all the different elements in the game.
- A governance based game meta decisions. With ths Sanctis modular system, anyone can develop a new module and integrate it in the universe, however, to allow it to interact with the rest of the community modules, it needs to be accepted by the community through a governance process. This means that most modules will maintain a community-validated state and a general state, to handle its acceptance by the community. This prevents for example grieffing, where a malicious modules steals all the resources from a player.
- A small fee is required to play. The fee itself is decided by the community, meaning it can evolve with the game's needs. The funds collected can then be used to finance development and marketing and other community initiatives. The membership also offers some in-game advantages. This also limits botting, as you can automate some part of the game but cannot scale to an unlimited number of account.