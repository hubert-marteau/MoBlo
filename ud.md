---
Title: MoBlo
Description: Modelization for BloCkChain Projects
article: Unit Definition
Keywords:
  - BlockChain
  - Modelization
  - MoBlo
  - Unit Definition
Contact Information: Hubert MARTEAU @ Worldline
License: CC BY-NC-ND 4.0
---

_The licence used for MoBlo articles is_ [_CC BY-NC-ND 4.0_](https://creativecommons.org/licenses/by-nc-nd/4.0/)

[**Return to Introduction**](/README.md)

[**Return to Global Architecture**](/ga.md)

# 4.    Unit Definition \(UD\)

Financial transactions are BlockChain transactions using crypto currencies. Crypto currencies are mostly used in financial projects.

Defined transactions are BlockChain transactions using units of asset or equivalent to define the nature of the content of the transaction.

Undefined transactions are BlockChain transactions only using additional data to send information which cannot be qualified.

## 4.1.    The Definitions

Definitions can specify the type of Assets which can be used and their cardinalities.

| Design | Description |
| :---: | :--- |
| ![](/Img/UD-ClosedAsset.png) | **Closed Asset** : The Asset is created with 500 units of it. No more units can be created; all the available units are created at the creation of the Asset. |
| ![](/Img/UD-OpenedAsset.png) | **Opened Asset** : The Asset is created with 500 units of it. This other cardinality indicates that units should grow by new request of 100 units. |

## 4.2.    Library use case UD

In the Population Map, we’ve seen that only the _Central Library_ was allowed to create _Assets_. Regarding the use case, three types of _Assets_ are necessary:

•    The first type of _Assets_ is “_New Book_”. This _Asset_ represents a lot of a same book. If the book has to be bought again later, then a new _Asset_ will be created because it won’t be the same lot. Then this _Asset_ is closed and the quantity is defined by the initial quantity of bought books.

![](/Img/UD-Library.png)

_**Figure 4-1 - UD - Library**_

•    The second type of _Assets_ is “_Booking_”. The units of this _Asset_ are used to represent the booking of a book by a reader in a specific Library. At first, the total number of booking can’t be defined and then the _Asset_ stays opened.

•    The last type of _Asset_ is “_Delay_”. The units of this _Asset_ are sent to _Readers_ to notice them that they are late. As for _Booking_, the total number of _Delay_ can’t be initially defined and then the _Asset_ stays opened.

_Please take care in the notation of Assets in UD. For “Booking” and “Delay”, the Assets are declared only one time at the initialization of the platform and after, units of the Assets are used. For “New Book i”, the letter “i” informs that fewer Assets can be created, for example let’s assume that an Asset “Ubik” is created with a quantity of 5, an Asset “H2G2” is created with a quantity of 42, …_

## 4.3.    Forum use case UD

The Forum is used to publish new subjects and comments related to the subjects.

![](/Img/UD-Forum.png)

_**Figure 4-2 - UD - Forum**_

A new subject can be created by the _Forum Creator_ or any member with the _Editor_ status. The units of the same _Asset_ are used to send a comment on the subject.

Here is the use case in a “perfect world”. Other Assets could be imagined like a “_Warning_” or “_Information_” ones.

[**Go to Business Transactions**](/bt.md)

