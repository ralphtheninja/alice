Alice
=====

This is an open source README project for facilitating communication of different aspects around developing software in the bitcoin community and the goal is to provide a collection of resources to developers working within the bitcoin economy.

This document is a story about a fictitious character, Alice, and tries to gather some of the endevours she might encounter while developing her business. Feel free to come up with your own sub stories of Alice's life and lets help her solve some of her problems, within a bitcoin context. Also feel free to use the issues page to discuss crazy future scenarios and further development of this document. Obviously, many of the things mentioned below can apply to any type of business and doesn't necessarily have to do with programming and similar activities.

The Story
---------

Alice wants to start her own business. She's a developer and would like to pay for the services she use in order to run her business as frictionless as possible. She also wants to have control of her privacy and not give out credit card numbers or other data she's not comfortable sharing.

###Wallets

While brainstorming she came to the conclusion that the most important thing to start with was to get herself a wallet. Without some form of wallet, even though it might be very basic in the beginning, she can neither get paid nor pay for her expenses. It seemed reasonable to fix this thing first. Wallets are usually divided into four groups: software wallets, hardware wallets, mobile wallets and web/online wallets.

* [blockchain.info](http://blockchain.info)

	One of the biggest and most reliable online wallets. They passed 500,000 wallets at the end of October 2013. Enables you to pay and get paid in bitcoins, using the browser on your desktop, or apps for both Android and iPhone. This means Alice can use pretty much any device she can get her hands on.
  
  Apart from the online wallet they also have a huge [API](https://blockchain.info/api). This means Alice could build her own tools or products integrating with bitcoin. Essentially, Alice could create her own system for book keeping which could automatically pay her bills and also issue payments to her customers.
  
  The API is split into:
  
  * [Receive Payments API](https://blockchain.info/api/api_receive)
  
  	Create receiving addresses with a HTTP GET. Very useful if you want to create new payments and serve customers with addresses they should pay to. When a payment has been made, the bitcoins will be transferred to an address of your choice. Also, you can provide an HTTP callback, which will be called once a payment has been completed.
  
  * [Blockchain Wallet API](https://blockchain.info/api/blockchain_wallet_api)
  
  	More advanced API for making payments, many transactions, managing addresses and all sorts of goodies. Also based on HTTP GET and also have a HTTP callback system.
    
  * [bitcoind/bitcoin-qt JSON RPC API](https://blockchain.info/api/json_rpc_api)
  
  	This API enables even more fine grained communication and gives access to the core of the bitcoin protocol by communicating with a *bitcoind/bitcoin-qt* process by utilizing JSON RPC. You can call almost all methods in the bitcoind json rpc api except for some that are disabled for security reasons.
    
    Alice could obviously setup her own *bitcoind/bitcoin-qt* process and enable this API without using blockchain.info, but this might be a good start if you don't want to invent everything yourself before getting started.
    
  * [Create Wallet API](https://blockchain.info/api/create_wallet)
  
  	Create new blockchain wallets programmatically.
    
  * [Blockchain Data API](https://blockchain.info/api/blockchain_api)
  
  	Get block and transaction meta data, block height, address data and other goodies.
    
  * [Query API](https://blockchain.info/q)
  
  	Various data and statistics on the blockchain and parameters in the bitcoin protocol, such as current block reward, current difficulty and things like that.
    
  * [Websocket API](https://blockchain.info/api/api_websocket)
  
  	Realtime notifications on new transactions and blocks.
    
  * [Exchange Rates API](https://blockchain.info/api/exchange_rates_api)
  
  	Market prices and exchange rates API (TODO: Find out the exact source of this data. Is it MtGox or something else?)  
  	
  * [Charts & Statistics API](https://blockchain.info/api/charts_api)
  
  	Provided access to the data used in any of the charts on the [Charts page](https://blockchain.info/charts).
    

* [CoinBase](https://coinbase.com/)

	TODO


###Finding Customers

Alice finally managed to get some customers that are willing to pay her in bitcoins, but boy was it hard to find them. Luckily she wrote down a list of different sites trying to connect people that want to do business in the bitcoin world:

* [r/Jobs4Bitcoins](http://www.reddit.com/r/Jobs4Bitcoins/ "r/Jobs4Bitcoins")

	Enables you to post if you're either [HIRING] or [FORHIRE]. There are also bounties offered for various things. Updates daily!

###Crowdfunding

Crowdfunding as part of the business model? Why not? If you can launch your own product it can create a more steady flow of income, which makes the business model more predictable and less chaotic. However, since creating a product involves a cost, crowdfunding can be used to mitigate those costs and perhaps even completely fund a project. This is a good alternative to Venture Capital, which might not be possible because you can't find anyone wanting to invest in you. With bitcoin it's easier to find peers that will believe in you and are willing to donate some bitcoin to make that happen.

* [BitcoinStarter](https://bitcoinstarter.com/)
	
  TODO

*	[Pozible](http://www.pozible.com/)

  TODO

###Hosting

Alice made an analysis of her customer base and found out it's varied in many ways. There is a flora of programming languages, operating systems, databases etc. However, the majority do need some form of hosting for e.g. a webservice or some other type of online service. Many are also ok with Alice being in charge of the hosting as well, they just need the services to be up and running and are willing to pay for the whole deal.

TODO List of different hosting services that accepts bitcoin.

###DNS

TODO

* easydns

###VPN

TODO

* ipredator
* mullvad
* purevpn
* bluevpn

###Point of Sale systems (POS)

Some of Alice's customers are running brick and mortar businesses and need her help setting up a Point of Sale (POS) system in order to start accepting bitcoin. Also, they might be merchants she need in her daily life, for example to buy food for both her and her dog Jazon. If she want to convince businesses in her everyday life to start using bitcoin, what POS system can she introduce to them to get them started as frictionless as possible?

* [blockchain.info](https://blockchain.info/)

	blockchain.info could be used as a POS system and is probably the way to go if you just want to set something up quickly and isn't necessarily interested in invoices or converting your bitcoins to fiat. If you just want to get up and running, this is currently the easiest way to do it. A variety of combinations can be made between mobile apps on Android or iPhone, or just running a browser in your mobile phone or if you have access to a surf pad even better. There is support for QR codes so it's easy for the other part to scan with their e.g. their smart phone.

* [BitPay Payment Gateway API](https://bitpay.com/bitcoin-payment-gateway-api)

	BitPay allows merchants to accept both bitcoins and/or fiat at the same time. Alice could actually use BitPay herself for selling her products and services. Perhaps she wants to monetize some online content and provide on the demand data with ease. Their pricing model is either fixed rate monthly payments with unlimited transactions and increasing support levels, which is good if you have an online store and deal only in bitcoin.
  
  However, if you're a small business bitcoin is probably going to be a small fraction of it, at least in the beginning. Therefore a monthly rate will not be economically sound since you could just continue using credit cards, but for this purpose BitPay also offer a percentage rate where you pay 1% of all your transactions. This is probably the way to go if you're a small business and just want to get going with bitcoin.
  
  BitPay has support for 30+ currencies and if you're an online store, already selling stuff for fiat money and have some sort of [shopping cart plugin](https://bitpay.com/bitcoin-shopping-cart-plugins), then BitPay can very easily be integrated with.
  
###Community

Naturally, since Alice is a hardcore bitcoin geek, she likes to keep her well informed on what goes on in the bitcoin community. She found that there are many channels to tap into, in form of youtube films from various conferences, online video tutorials, pod casts, blogs etc.

* [Lets Talk Bitcoin](http://letstalkbitcoin.com/)

	This is currently by far the best podcast on everything surrounding bitcoin. It's a twice weekly audio show by [Adam B. Levine](https://twitter.com/GamerAndy) and his eminent co-hosts [Stephanie Murphy]( "TODO Link missing") and [Andreas M. Antonopoulos](https://twitter.com/aantonop). It's also a very nice blog with contributions from other people in the bitcoin community and if you think an article is interesting you can tip in bitcoin directly to the author.

* [Bitcoin or How I Learned to Stop Worrying and Love Crypto](https://www.udemy.com/bitcoin-or-how-i-learned-to-stop-worrying-and-love-crypto)

	Awesome video tutorial made out of many different videos describing most of the things revolving bitcoin. From the most basic to how you can use paper wallets to increase security to tutorials on different wallets, how mining works and much more. Most of the videos are made by Charles Hoskinson (mathematician behind [BitShares](http://invictus-innovations.com/) and also [The Bitcoin Education Project](http://btcedproject.org/)) but there are also contributions made by [Jon Matonis](https://twitter.com/jonmatonis).

###Traveling

Alice like to put aside some money so she can travel on a regular basis. There will probably be business trips and also trips on vacations. Not to mention, Alice is involved in several communities and often attend several conferences each year to keep up with what's going on. This is especially the case if you are into Open Source, which you probably are if you're reading this.

Going somewhere for an extend period of time means Alice has to find places to stay as well. Her demands aren't that high so she can accept staying in a cheaper hotel, airbnb and perhaps even a hostel, if it's a nice place.

TODO List of travel agents etc


###Distributed/Decentralized Autonomous Corporations (DACs)

Alice and her friend Bob have realized they have several things in common. Some of their customers have use for the same functionality, so Alice and Bob start a Distributed Autonomous Corporation. The company has shares in bitcoin and everyone invested in the project can share the profit and obviously also the costs, which spreads out risk over multiple parties. This could be implemented as a DAC. In fact the entire bitcoin economy could be looked upon as a DAC, where owners of bitcoin own shares in the bitcoin economy.

Since Alice follows the completely badass online paper [Bitcoin Magazine](http://bitcoinmagazine.com/), she obviously already read the article series on [Bootstrapping A Decentralized Autonomous Corporation: Part I-III](http://bitcoinmagazine.com/7050/bootstrapping-a-decentralized-autonomous-corporation-part-i/) by Vitalik Buterin and of course also [Bitcoin and the Three Laws of Robotics](http://letstalkbitcoin.com/bitcoin-and-the-three-laws-of-robotics/#.UnApcrOOO1Q) by Stan Larimer.

Contributors
------------

If you contribute to this README project you will be given commit access to this repository and end up on the list below. Obviously only if you want to :)

<table><tbody>
<tr><th align="left">Lars-Magnus Skog</th><td><a href="https://github.com/ralphtheninja">GitHub/ralphtheninja</a></td><td><a href="http://twitter.com/ralphtheninja">Twitter/@ralphtheninja</a></td></tr>
</tbody></table>


License
-------

MIT