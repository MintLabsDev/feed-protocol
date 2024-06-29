<picture>
  <img alt="feed protocol banner" src="./banner.jpeg" width='925'>
</picture>

# Feed Protocol RNG

Feed Protocol Random Number Generator (FPRNG) is a program on the Solana Blockchain to derive on-chain randomness. You interact with FPRNG (making a CPI) in your program to get randomness and use it in the same transaction. FPRNG's pricing advantage allows you to significantly scale randomization in your programs. FPRNG takes advantage of the speed and security of the Solana Blockchain to offer cheap, fast, unpredictable, and fair random numbers.

When a user gets a random number from FPRNG, they manipulate the process to derive randomness for the next user and also for themselves. Additionally, feed data from Pyth Network accounts, timestamp, slot number, and a temporarily created account are used in a complex process to derive randomness.

The advantage of the FPRNG is that you can handle the derived random number in only one transaction. Let's say you make a game where opponents hit each other in turns, and the damage they inflict on the opponent is random. In your play function, you make a CPI to FPRNG, and again in the same function, FPRNG returns to you a random number that you can use in the same function. This provides users with a seamless game experience. You don't need to create callback functions or store this randomness in an account to use it.

FPRNG also uses native SOL coin for charging. You don't need to subscribe or use any other tokens to use FPRNG. The technology of the Solana Blockchain allows FPRNG to be very cheap and fast.

FPRNG is very easy to implement. You can take a look at example programs in the links provided.

## How to Use

1. Use program id to set FPRNG. Devnet, Testnet, Mainnet Beta and [Mainnet](https://solscan.io/account/9uSwASSU59XvUS8d1UeU8EwrEzMGFdXZvQ4JSEAfcS7k) addresses are the same as below
```
9uSwASSU59XvUS8d1UeU8EwrEzMGFdXZvQ4JSEAfcS7k
```

2. Set offsets and accounts
3. Call InvokeRNG method
4. Now you can use your random number

## Examples

 - [Coin Flip Solana Example](https://github.com/MintLabsDev/coin-flip-solana-example)
 - [Coin Flip Unity Example](https://github.com/MintLabsDev/coin-flip-unity-example)
 - [Coin Flip Anchor Example](https://github.com/MintLabsDev/coin-flip-anchor-example)

## Resources

 - [Audit Reports](./feed-protocol-public.pdf)
 - [Mint Labs Github](https://github.com/orgs/MintLabsDev)
 - [Protocol Deck](https://www.canva.com/design/DAGJgAPXgwM/-QXEVdOMUciOe-tsAw9W9w/edit)

---

[![Twitter](./mail.png)](mailto:hello@mintlabs.dev) [![Mail](./twitter.png)](https://x.com/feed_protocol) 

Powered by [Mint Labs](https://mintlabs.dev/)