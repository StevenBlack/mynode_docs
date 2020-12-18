# Dojo
## What is it?
In order to better answer this question, we should first look into what **Light Wallets** are and how they work.

**Light Wallets** are a type of wallet that can run on devices with limited amounts of storage capacity and RAM, such as a mobile phone for example. Any and all bitcoin wallet apps you find in the google or apple stores are light wallets. These are wallets that don't contain the blockchain themselves, yet they are able to send and receive bitcoin, as well as to show the current balance of a wallet. The reason why they are able to operate and show all this info is because **Light Wallets**  connect to a **Full Node** at some point to gather all this data. There are many ways in which this connection can be done ([Transaction Bloom Filters](https://bitcoinops.org/en/topics/transaction-bloom-filtering/), [Xpub Sharing](https://support.cryptfolio.com/i227-is-there-a-risk-when-sharing-xpub-keys)...) and while some are more private than others, in one way or another they all end up providing information about your wallet to whoever controls this **Full Node**.  

**Full Nodes**, such as myNode, contain every transaction anyone ever made in the bitcoin blockchain. All the information needed to show a balance on a wallet can be gathered from here, hence the dependency of **Light Wallets** on them. The most private way of making a **Light Wallet** get this info is by hosting a **Full Node** yourself and connecting them to one another. This way, you phone wallet will connect to your own node and you will not be leaking private information to untrusted third parties.

**Dojo** is Samourai Wallet's solution to address this. By running **Dojo** in your myNode, you can connect your phone's Samourai Wallet to it - this way your Samourai **Light Wallet** will request information about your account balance and transactions to your own personal **Full Node**. No one will know what your past, current or future addresses are, since you won't be sharing your [Xpub](https://support.samourai.io/article/49-xpub-s-ypub-s-zpub-s) with anyone.