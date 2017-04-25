_The licence used for MoBlo articles is_ [_CC BY-NC-ND 4.0_](https://creativecommons.org/licenses/by-nc-nd/4.0/)

[**Return to Context**](/context.md)

# 2.    Population Map \(PM\)

This is a first step to define the perimeter of a BlockChain project: what are the rights of actors for the project.

## 2.1.    The Rights

Here are listed possible rights that can be found in a BlockChain project.

Rights are defined here for the following nodes of the network.

|  |  |
| :---: | :--- |
| ![](/Img/SimpleNode.png) | **Simple Node** : Node not able to connect to the BC |
| ![](/Img/OriginNode.png) | **Origin Node** : Creator of the BC _\(Naturally has admin rights\)_ |
| ![](/Img/Admin.png) | **Admin** : Can give and revoke to anyone the rights : issue, mine, activate, admin, connect, send receive |
| ![](/Img/Activator.png) | **Activator** : Can give and revoke to anyone the rights : connect, send, receive |
| ![](/Img/Miner.png) | **Miner** : Node processing blocks of the BC |
| ![](/Img/Connect.png) | **Connect** : Node able to connect to the BC |
| ![](/Img/Send.png) | **Send** : Node able to send new transaction to the BC _\(Necessarily able to connect\)_ |
| ![](/Img/Receive.png) | **Receive** : Node able to receive transaction in the BC _\(Necessarily able to connect\)_ |
| ![](/Img/Issue.png) | **Issue** : Node able to create new asset in the BC _\(Necessarily able to connect and receive\)_ |

## 2.2.    Library use case PM

In the Library use case, there are 4 kinds of actors:

* The _Central Library_

* The others _Libraries_

* The _Readers_

* Other _Actors _\(not linked to library system\)

All the rights can be represented by the next figure:

![](/Img/PM-Library-Ext.png)_**Figure 1 - Population Map - Library - extented**_

Let’s take again each actor with their rights:

* The _Central Library_:

  * It is the BlockChain **Creator**
  * It has **Admin** rights on the BlockChain
  * It has **Activation** rights on the BlockChain
  * It is a **Miner**
  * It can **Connect** to the BlockChain
  * It can **Send** transactions in the BlockChain
  * It can **Receive** transactions in the BlockChain
  * It can **Issue** in the BlockChain

* The others _Libraries_:

  * They have **Activation** rights on the BlockChain
  * They are a **Miner**
  * They can **Connect** to the BlockChain
  * They can **Send** transactions in the BlockChain
  * They can **Receive** transactions in the BlockChain

* The _Readers_:

  * They can **Connect** to the BlockChain
  * They can **Send** transactions in the BlockChain
  * They can **Receive** transactions in the BlockChain

* Other _Actors_ \(not linked to library system\):

  * They cannot connect!!! Then they cannot read information.

But in this list, a few rights are redundant.

If you are able to write in a BlockChain, then you inevitably have the right to connect. Similary, the creator of a BlockChain has Admin and Activation Rights.

_Notice: it’s a good way to keep highlighted status rights, process right and business rights._

Then the list can be reduced in:

* The _Central Library_:

  * It is the BlockChain **Creator**
  * It is a **Miner**
  * It can **Send** transactions in the BlockChain
  * It can **Receive** transactions in the BlockChain
  * It can **Issue** in the BlockChain

* The others _Libraries_:

  * They have **Activation** rights on the BlockChain
  * They are a **Miner**
  * They can **Send** transactions in the BlockChain
  * They can **Receive** transactions in the BlockChain

* The _Readers_:

  * They can **Send** transactions in the BlockChain
  * They can **Receive** transactions in the BlockChain

* Other _Actors_ \(not linked to library system\):

  * They cannot connect!!! Then they cannot read information.

Thus, the rights can be represented by a compact version of the figure:

![](/Img/PM-Library-Compact.png)_**Figure 2 - Population Map - Library - Compact**_

## 2.3.    Forum use case PM

In the Forum use case, there are 4 kinds of people:

* The _Creator of the forum_

* The _Editors_ \(with the right to create new topics\)

* The _Subscribed Readers_

* The \(Simple\) _Readers_

All the rights can be represented by the next figure:

![](/Img/PM-Forum.png)_**Figure 3 - PM - Forum**_

The figure represents the compact version of the Population Map \(PM\).

The rights are defined following rules to show another aspect of rights.

The list of rights is the following one:

* The _Creator_ of the forum:
  * It is the BlockChain **Creator**
  * It is a **Miner**
  * It can **Send** transactions in the BlockChain
  * It can **Receive** transactions in the BlockChain
  * It can **Issue** in the BlockChain
  * It can **Receive** on another address.

_Notice: The forum has a wall, an editorial line. A specific address is created just to receive the posts. It is possible to imagine that editors could have their own address and that the forum would have then few editorial lines. In fact, technically, if you can receive transactions then you can create your own editorial line. Note that, above all, the Forum Creator is represented with two statuses: one is full of rights, it is its user status; the other one can only receive rights, it is the editorial line._

_Notice: An address with only “receive” right can be considered like a publication wall \(a discussion later compare transactions and streams for this use case\)._

* The _Editors_ \(having rights to create new topics\):

  * It can **Send** transactions in the BlockChain
  * It can **Receive** transactions in the BlockChain
  * It can **Issue** in the BlockChain

* The _Subscribed Readers_:

  * They can **Send** transactions in the BlockChain
  * They can **Receive** transactions in the BlockChain

* The \(Simple\) _Readers_:

  * They can **Connect** and then read \(and only read, the posts.

## 2.4.    Particular case: Multi-Signature

In few cases, it can appear necessary to use multisign addresses. A multisign address is an address which can be signed by \(p\) different pub keys and which has to be signed by \(s\) signatures. Then, a multisign address is noticed with \(s x p\) to inform that \(s\) signatures are needed in the \(p\) possible pub keys.

In Population Map, this is represented with a new box and the signature format.

![](/Img/PM-MultiSig.png)

_**Figure 4- PM – MultiSign Addresses**_

In this figure, there are two addresses shared by Alice and Bob:

•    the first can send transactions only with one signature \(Alice’s signature or Bob’s signature\),

•    the second to send transactions need two signatures \(Alice’s signature and Bob’s signature\)

_Notice that few screens have to be used when there are different crossed multisign addresses: when one address is 3 x 6 and, in the same use case, another is 4 x 5, and another is … The goal of the Population is to be clear, then different screens can be used to represent the population._

## 2.5.    Particular case: Import of Private Key

In few cases, it can appear necessary to import the private key of a wallet from to another one. Then the second one receives all the rights of the first one and can act as the first one. It has to be done with a lot of precautions.

In PM, this is represented with a simple arrow.

Figure 5- PM - Import of Private Key

In this figure, Bob can create an Issue in the BlockChain and Alice cannot do it directly, but Alice has the control of a Bob’s wallet address, then Alice can create an Issue using Bob’s rights on this address.

Technically, it means that Alice imported the private key of one of Bob’s addresses.

[**Go to Global Architecture**](/ga.md)

