👋 Hi, I’m @x0rswap. Looking for solidity contracts. Ping me on twitter: https://twitter.com/xor_swap

Here are some small projects that show I know the basics: I know how to write a simple contract, a simple dApp, a simple CI with some tests, ...  


## May the CI be with you

https://github.com/x0rswap/may-the-CI-be-with-you

Just a CI that fuze a contract which contains an overflow. Sometimes the CI finds the overflow, sometimes no.  
You can see the last commit failed, but the commit just before was successful, even if only the readme has been changed.  
Built with foundry.

## Solidity x MNIST

https://github.com/x0rswap/Solidity-x-MNIST

The goal at first was to build a neural net that allow you to mint an NFT iif it considers it's a picture of "pipe".  
(People would then build GANs to trick the neural net and mint cool NFTs ^-^)

![](https://upload.wikimedia.org/wikipedia/en/b/b9/MagrittePipe.jpg)

So I first tried with MNIST, and it's already a nightmare, and would be unsable on mainet anyway.  
So you can find the jupiter notebook that trains a neural network for MNIST, export it, and then a solidity file which computes a prediction.  
(The type used is tf.float32, so I wrote also a fixed point library, and I've checked with the notebook I get almost the same result).

`forge test` takes 10min to compile the file. Too much line. I couldn't export the full model, so only exported the important parts.  
(With less parts it can take like 1min but the accuracy is really ridiculous)

Accuracy of the model: 60% 😂

Thinking about launching a rollup focused on machine learning 😂  
A simple matrix computation shouldn't be a problem for an OR anyway, the code to store is ridiculous, and tensorflow computes it really fast.

Anyway, this project could be improved a lot, but won't ever be usable on mainet imo so ...

## The end


📫📫 Follow me on twitter: https://twitter.com/xor_swap 📫📫
