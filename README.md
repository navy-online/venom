# Venom hackathon summary

Hello, this is the navy-metaverse.online team.
Our project is a metaverse game about naval battles, ships and islands.

On this page we want to give a brief information about the work done during the Venom hackathon.
Firstly, our project has already won the hackathon from Cronos, where we took first place. At that time, we focused on the basic gameplay and the overall vision of the project, you can get acquainted with the result and the gameplay record by following the link:
However, during the Venom hackathon, we decided to turn our project as ready as possible to launch and attract investment, so we concentrated on creating a community, promotional materials, and also created our own marketplace, which is the main development of the hackathon. Unfortunately, we did not have time to add venom to our game client, and we will not demonstrate it =(

# Briefly about what we have done in a month:

1) New landing page - https://navy-metaverse.online

2) White paper - https://navy-metaverse-online.gitbook.io/navy.online-whitepaper/intro/about-navy-metaverse.online

3) Pitch - https://docs.google.com/presentation/d/1UxntuujawPg0awNYnO5_7WPJVvxzWzZtG1tydpZl440/edit#slide=id.g242ec781acd_0_0

4) Social media:
https://twitter.com/_NavyOnline_ 
https://t.me/navy_online_game
https://mastodon.social/@_Navyonline_
https://zealy.io/c/navymetaverse/questboard

5) Crosschain marketplace with minting functionality -
https://marketplace.navy-metaverse.online

6) Made a small patch for Venom Wallet =)

# Technical part

Our backend is micro-service, most of the work on the backend was to create a convenient abstraction for working with both evm-like and ton-like blockchains.

Services to check:

1) web3-service
This service listens for all kind of new web3 events (minting, marketplace sales, etc), and wraps this event as a queue job
https://github.com/navy-online/NavyOnline/tree/venom-hackathon/server/navy/apps/web3-service

2) web3-worker-service
This service is responsible for processing web3 related jobs 
https://github.com/navy-online/NavyOnline/tree/venom-hackathon/server/navy/apps/web3-worker-service

3) marketplace-service
This service provides an api for marketplace frontend
https://github.com/navy-online/NavyOnline/tree/venom-hackathon/server/navy/apps/marketplace-service

# All repos:

https://github.com/navy-online/NavyOnline (switch to venom-hack branch. it contains both game client and server)
https://github.com/navy-online/navy-online-contracts (project is separated by cronos and venom, each has contracts, tests, deploymets scripts and samples (venom has both client and server sample))
https://github.com/navy-online/navy-online-marketplace
https://github.com/navy-online/navy-online-landing
