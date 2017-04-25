_The licence used for MoBlo articles is_ [_CC BY-NC-ND 4.0_](https://creativecommons.org/licenses/by-nc-nd/4.0/)

[**Return to Introduction**](/README.md)

[**Return to Population MAP**](/context.md)

# 3.    Global Architecture \(GA\)

When population is defined, a global architecture needs to be defined. This architecture allows defining how each application interacts with the BlockChain. It allows then to explicitly present external services to implement.

## 3.1.    Architecture elements

See below the elements to define the global architecture.

| Design | Description |
| :---: | :--- |
| ![](/Img/GA-BC.png) | **BlockChain** : Representation of the BlockChain grouping together all the nodes. |
| ![](/Img/GA-ExtServ.png) | **External Service** : Representation of an external service that needs to access to information. |
| ![](/Img/GA-Application.png) | **Application** : Application used by someone of the population. |
| ![](/Img/GA-Link.png) | **Link** : Link between the nodes and the population. |

## 3.2.    Library use case GA

In the Library use case, the libraries have an interest to be directly connected to the BlockChain.

_Readers_ don’t have to install or configure anything to use the system. Then a Web Gate has to be implemented to let them use the service. Another reason of the gate is the lack of interest for _Readers_ to possess all the data. Regarding Population Map, _Others_ don’t have any right to connect to the BlockChain, and then the Web Gate needs to have a restricted access.

In complement of the Population Map, batches are necessary to create and send delay-related mail to _Readers_ for example or manage the books to send from a library to another one.

![](/Img/GA-Library.png)

_**Figure 3-1 – GA - Library**_

The figure represents the 3 nodes with rights inside the BlockChain. The interfaces of _Central Library \(CL\) and Libraries \(L\)_ are directly connected to the BlockChain. _Readers_ use a Web Gate to communicate with the BlockChain. Batches are using the _Central Library_’s address to access to the BlockChain.

## 3.3.    Forum use case GA

The goal of the Forum is to discard all the web tools. Except to send and receive information in using transactions, there are no specific cases to identify. The goal of the forum which is a wall of publications is to maintain it completely open to everyone.

![](/Img/GA-Forum.png)

_**Figure 3-2 - GA - Forum**_

## 3.4.    Particular case: Batch & SmartContract

In the particular of multiSig addresses the Global Architecture allows to define explicitly the related pub keys.

![](/Img/GA-MultiSig.png)

_**Figure 3-3 - GA - MultiSig**_

In the figure Alice uses one address with one multiSig address \(M1\) and her other address with the other multiSig address \(M2\).

Labels are added to the multiSig addresses to distinguish them later just in using this label.

## 3.4.    Particular case: Multi-Signature

In the particular of multiSig addresses the Global Architecture allows to define explicitly the related pub keys.

![](/Img/GA-MultiSig.png)

_**Figure 3-3 - GA - MultiSig**_

In the figure Alice uses one address with one multiSig address \(M1\) and her other address with the other multiSig address \(M2\).

Labels are added to the multiSig addresses to distinguish them later just in using this label.

[**Go to Unit Definition**](/ud.md)

