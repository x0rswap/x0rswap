👋 Hi, I’m @x0rswap. Learning solidity atm. Ping me on twitter: https://twitter.com/xor_swap

Here are some small projects that show I know the basics: I know how to write a simple contract, a simple dApp, a simple CI with some tests, ...  


## May the CI be with you

https://github.com/x0rswap/May-the-CI-be-with-you

Just a CI that fuze a contract that contains an overflow. Sometimes the CI finds the overflow, sometimes no.  
You can see the last commit failed, but the commit just before was successful, even if only the readme has been changed.  
Built with foundry.

## I know how to copy paste

https://github.com/x0rswap/I-know-how-to-copy-paste

Copy pasted from https://github.com/buildspace/buildspace-projects/tree/main/Solidity_And_Smart_Contracts/en  
And modified of course.  
Just to show I can build a full web3 dApp from scratch by copy pasting code here and there.  
I guess ideally you'd want an infura API to list all messages instead of storing them directly in the contracts. Maybe one day.

Link to the app: https://waveportal-starter-project.x0rswap.repl.co (sorry it takes 5min to load, replit's fault not mine, and also it's on replit testnet not rinkeby)

<img src="https://cdn.discordapp.com/attachments/942545565663756378/942902241218674758/unknown.png" width="500"/>

Isn't it beautiful?  
I also wanted to make a probabilistic check for the prime number, but maybe one day too, will probably be hard to design something that cannot be gamed.

## Solidity x MNIST

https://github.com/x0rswap/Solidity-x-MNIST

The goal at first was to build a neural net that allows you to mint an NFT iif it considers it's a picture of "pipe".  
(People would then build GANs to trick the neural net and mint cool NFTs ^-^)

![](https://upload.wikimedia.org/wikipedia/en/b/b9/MagrittePipe.jpg)

So I first tried with MNIST, and it's already a nightmare, and would be unusable on mainet anyway.  
So you can find the jupiter notebook that trains a neural network for MNIST, export it, and then a solidity file that computes a prediction.  
(The type used is tf.float32, so I wrote also a fixed point library, and I've checked with the notebook I get almost the same result).

`forge test` takes 10min to compile the file. I couldn't export the full model (takes too long & `solc error`), so only exported the important parts.  
(With fewer parts it can take like 1min but the accuracy is really ridiculous)

Accuracy of the model: 60% 😂

Thinking about launching a rollup focused on machine learning 😂  
A simple matrix computation shouldn't be a problem for an OR anyway, the code to store is ridiculous, and tensorflow computes it really fast.

Anyway, this project could be improved a lot, but won't ever be usable on mainet imo so ...

## Prove you are good trader with NFTs

https://github.com/x0rswap/Are-you-really-a-good-trader

Root your uniswap trades through this contract to mint an exclusive non-transferable NFT that remembers, forever, at what price you bought.  
If you are a good trader, just leave the proof on chain :) inspired by https://twitter.com/ercwl/status/1467560841742635009

I used this https://github.com/lightcycleresearch/foundry-getcode/blob/master/try-v1/src/test/Contract.t.sol

## The MEV will claim it

https://github.com/x0rswap/Its-safe-the-MEV-will-claim-it

If you almost-never update a storage value, then just makes it an immutable value, read from it, and redeploy the contract each time you need to change it.

If you give away eth if it turns out the immutable isn't the storage, then someone will each time claim the bounty, right?

<img src="https://github.com/x0rswap/Its-safe-the-MEV-will-claim-it/blob/main/mem.jpg" width="500"/>

## The end


📫📫 Follow me on twitter: https://twitter.com/xor_swap 📫📫
