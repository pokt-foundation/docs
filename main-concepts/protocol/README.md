---
description: Protocol Introduction
---

# ⛓ Protocol

## Why does Pocket exist?

**Pocket network exists to solve 2 major issues** for 2 key participants of the decentralized web:

1. Pocket network allows developers to connect their applications to their blockchain of choice in a decentralized, private, cheaper and scalable manner \(yes, all that!\)
2. Pocket network creates a new source of revenue for node runners who are traditionally left aside in the incentive structure of most blockchains.

Let's dive more into each of these!

## **Why use Pocket as a developer**

Pocket network allows developers to connect applications to public blockchains \(and other public distributed systems like Airweave\) in a decentralized manner, without requiring them to host their own nodes.

### What's wrong with today's way of interacting with blockchains?

Let's start with the basics. At its core, **any blockchain network is made up of nodes** communicating together in a peer-to-peer \(p2p\) fashion in order to reach consensus around some shared data \(the blockchain\). In other words, not every computer connected to the internet can interact with a blockchain, only those running a program implementing the protocol of the blockchain considered \(1\). To be fully exact, this description of network of nodes also applies to distributed systems like Arweave which are not blockchains but share the same p2p and openess characteristics as blockchains.

This topography implies that developers of decentralized applications \(or dapps\) who don't run a node of their own must connect to a node run by a third-party to access the blockchain. Yet, the high requirements to run nodes and the operational hassle associated make it so that **most developers choose not to run their own nodes**.

The issue with this situation is that most provider of blockchain's nodes out there offer a centralized solution. Meaning the nodes they give developers access to are nodes of their own, managed and controlled exclusively by them. It's a problem because this **reliance on few select providers introduces back centralization**. What's the point of building a decentralized application if it's to interact with it in a centralized manner? It breaks the very reasons why developer build decentralized applications in the first place \(anti-fragility, censorship resistance, etc\).

### How is Pocket network injecting decentralization in the way dapps interact with blockchains?

Unlike centralized providers, **Pocket doesn't own, nor manage nodes**. Pocket network is a protocol that full node runners of various blockchains can choose to join against compensation. By joining Pocket, the node runners offer access to their nodes to developers of the Pocket network. The matching between application's requests looking to interact with a blockchain and nodes on that blockchain is done in a **trustless** manner through the Pocket protocol \(later sections of the documentation we refer to it as the "Network layer"\).

### What benefits does Pocket bring over centralized providers?

* **Resilience**. However well funded and competent its devops team, one centralized provider can always go down \(2\). Yet, it is less likely that the hundreds of independant node providers of Pocket go down all at once. If the ones an application is paired with fall, Pocket will route its requests to other nodes. No downtime.
* **Cost reduction**. Pocket creates an open market for node access. As anyone can provide a node to the network, access to node becomes commodized. Application developers no longer have to shop to a few select centralized node providers. This result in lower prices for app developers.
* **Censorship-resistance**. Pocket being a protocol, an algorithm, not a company, it doesn't have the discretion to censor certain users. It stays neutral.
* **Privacy**. Given that centralized services receive all the requests emitted by their client applications, they can easily aggregate those to track the activity on those applications. Developers have to trust they won't do so. On the contrary the privacy of Pocket is trustless. Application requests are frequently routed to a different set of nodes meaning that no node runner can build a profile of the activity of the application. Privacy is built-in.

Last but not least, not only is Pocket better than centralized providers but it is also better than running your own node. Putting aside it's **less hassle** for a developer, using Pocket network provides **elasticity** out-of-the box. Like anything, a node can only deal with so many requests before being saturated. By using Pocket, application developers can immediately scale their ability to meet incoming any influx of traffic.

**Head over to the Application developer section to learn how to use Pocket in your application!**

{% page-ref page="../../paths/app-developer/" %}

## **Why use Pocket as a node runner**

For node runners, the pitch is straightforward: Pocket network unlocks a **new revenue** stream without changing much to their existing operation.

### What's wrong for most node runners today in proof-of-work blockchains?

In most established proof-of-work \(PoW\) blockchains like Bitcoin or Ethereum \(1.0\), the **incentive structure for nodes comes from mining**, i.e. the reward node runners get when they solve the math puzzle of the chain, thus get to include a new block to the blockchain. The reward is made up of two elements: the coinbase, an amount of tokens that the miner receives when mining the block, as well as the sum of the fees of the transactions included in the new block. There's a probabilistic aspect to this, in that the more computing power the miner has the more likely he is to come up with the next block.

Yet **mining fails to compensate most node runners today**. At inception, the network of PoW blockchains are small enough so that most node runners have a fair chance to being picked as block creators. Yet as the blockchain grows in value, its network is joined by increasingly powerful nodes seeking to reap its rewards \(3\). Hobbyists and even professional participants not running their nodes on specialized hardware find themselves with a likelihood of finding the next block and getting rewarded for it close to zero \(4\).

Still, nodes remain essential to any PoW blockchain network. As explained in greater detail in the developer section above, they are needed to interact with the blockchain, to send transaction to the blockchain and read info from it. They are also important in that they enforce the consensus rules of the blockchain. They do so by only accepting and propagating transactions and blocks adhering to the standards of the blockchain.

### How is Pocket helping node runners of PoW blockchains?

When joining the Pocket network, **node runners get paid for the requests they serve** to application developers. These requests may be read or write requests.

Once Pocket is set up, node runners essentially don't do more than what they used to do running their nodes otherwise, except that now they get paid for doing what they did for free.

**Head over to the Node runner section to learn how to set-up Pocket in your application!**

{% page-ref page="../../paths/node-runner/" %}

{% hint style="info" %}
**TODO: Add a sub-section for Proof of stake blockchains.**
{% endhint %}



Notes:

\(1\) For example, [geth](https://github.com/ethereum/go-ethereum) is a popular node program allowing the computer running it to become part of the Ethereum network.

\(2\) Infura, the largest node provider owned by Consensys, went down on November 11th 2020 resulting in major disruption on Ethereum as many distributed applications rely on it to access Ethereum \([src](https://coinmarketcap.com/alexandria/article/ethereums-infura-iating-outage-revives-decentralization-concerns)\)

\(3\) The last stage of this evolution being the introduction of machines with specialized hardware specifically designed to run the consensus algorithm of the blockchain as efficiently as possible. [Examples of specialized hardware for Bitcoin](https://www.buybitcoinworldwide.com/mining/hardware/).

\(4\) Joining a pool of miners, which share the work and profit of mining, doesn't change much for miners running on non-specialized hardware. Large bitcoin pools even discourage people to join when mining on non-specialized hardware. That's the case for the Slush pool for example \([src](https://help.slushpool.com/en/support/solutions/articles/77000422800)\).



