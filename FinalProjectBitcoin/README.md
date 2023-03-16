Bitcoin is a decentralized digital currency that enables peer-to-peer transactions without the need for intermediaries such as banks or governments. Bitcoin operates on a decentralized ledger called the blockchain, which is a continuously growing list of records or "blocks" linked together and secured using cryptography. Each block in the chain contains a record of several transactions, and once a block is added to the chain, it cannot be altered. 

I have written some Python code which demonstrates how a blockchain works using PythonThe Wallet class is used to generate a public-private key pair for a wallet, which can be used to send and receive transactions. The Transaction class represents a single transaction, including the sender and recipient addresses and the amount being transferred. The Block class is used to group transactions together into a block, which is then added to the blockchain. The Blockchain class is responsible for maintaining the blockchain and handling transactions, including mining new blocks and validating transactions. This code demonstrates how the blockchain uses cryptography to secure and validate transactions, and how new blocks are added to the chain through a process called mining, which involves solving a cryptographic puzzle.


Bitcoin stores its blockchain through a distributed network of nodes that collectively maintain a copy of the entire blockchain. Each block in the blockchain contains a cryptographic hash of the previous block, forming a chain of blocks that cannot be altered without also changing all subsequent blocks. In my code, the blockchain class serialises the chain to a JSON string and writes it to a file.

You can view my blockchain code and interact with it here: 


Now we understand what Bitcoin is and how it works, 

The next part of my project was to use machine learning to predict the price of Bitcoin.

The first part of this project was exploring the features that i would use in my model. I sourced data from a variety of sources that were linked to Bitcoin. 



![ds](/images/btc_ds.jpg)
We can see here that there is some relationships between dollar strength and the price of Bitcoin. As the dollar began to weaken in March 2020, Bitcoin gan to rally. And as the dollar began to regain strength in July 2021, Bitcoin sold off. The sharp increase in dollar strength in November 2021 also coincided with the beginning otf the recenet bitcoin bear market. 


![et](/images/btc_eth.jpg)
We can see in this graph that the price of Bitcoin is highly correlated with the price of the second largest cryptocurrency, Ethereum .


![tb](/images/btc_tb.jpg)
We can see here that there is a strong negative correlation between the price of Bitcoin and the interest rate on 1-Year Treasury bonds. 16



![ns](/images/btc_ns.jpg)
We can see here that Bitcoin is also highly correlated with the Nasdaq 100, an index of 100 of the largest technology companies in the US.



![ts](/images/btc_ts.jpg)
This chart plots the price of Bitcoin with the sentiment of tweets related to Bitcoin. 

![sv](/images/btc_sv.jpg)

This graph plots the price of Bitcoin with total social volume, which is the bitcoin content across all social platforms. We can see that it follows the trend of the price.



