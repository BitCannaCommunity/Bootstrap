# Bootstrap
Bootstrap.dat is a file that contains the copy of blockchain from genesis block to a certain point of time. This compressed Bootstrap.dat file is used to speed up the initial blockchain download times

# Instructions
* 1.Download from github: https://github.com/BitCannaCommunity/Bootstrap/releases/download/0_300K/bootstrap300k.zip
* 2.Unzip.
* 3.Close your BitCanna node
* 4.Copy the bootstrap.dat file in the "\user\AppData\Roaming\BCNA" folder,  NOT in the "\user\AppData\Roaming\BCNA\blocks" folder.
* 5.Run your BitCanna node again, it should start 'syncing from disk'

# How it works? 
Your wallet client downloads and verifies each blocks from the P2P network. This is usually slow and especially if you are using wallet for the first time then syncing process can take quite a long time.

Instead of using Peer to Peer communication your wallet client can read blockchain data from this compressed bootstrap file which contains the copy of blockchain data until a certain block height. Once the wallet client completes reading data from bootstrap file, it will then use the P2P connection to download the remaining blocks. This method is faster and moreover it consumes less bandwidth compared to standard synchronization process. However still bootstrap method takes some time as your wallet client needs to validate each individual blocks.
(source: https://coinguides.org/bitcoin-bootstrap-dat-source-usage/)

# Can I trust in this Bootstrap?
Yes you can, the offical BitCanna Announcement was on xx/xx/xxxx at this media:
* https://.......
