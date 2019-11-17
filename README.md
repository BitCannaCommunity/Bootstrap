# Bootstrap
Bootstrap.dat is a file that contains a copy of the blockchain from genesis block to a certain point in time. This compressed Bootstrap.dat file is used to speed up the initial blockchain download time, but it will still validate all the blocks which takes time. 
It definitely is faster than downloading it from scratch.
 
We will provide a new bootstrap every 4-6 weeks after the latest release! 

# Instructions
* 1.Download from github: https://github.com/BitCannaCommunity/Bootstrap/releases/download/bootstrap/bootstrap.zip
* 2.Unzip
* 3.Close your BitCanna node
* 4.Copy the bootstrap.dat file in the "\user\AppData\Roaming\BCNA" folder,  NOT in the "\user\AppData\Roaming\BCNA\blocks" folder.
* 5.Run your BitCanna node again, it should start 'syncing from disk'

# How it works? 
Your wallet client downloads and verifies each block from the P2P network. This is usually slow and especially if you are using the wallet for the first time, then syncing process can take quite a long time.

Instead of using Peer to Peer communication your wallet client can read blockchain data from this compressed bootstrap file which contains a copy of the blockchain data until a certain block height. Once the wallet client completes reading data from bootstrap file, it will then use the P2P connection to download the remaining blocks. This method is faster and moreover it consumes less bandwidth compared to standard synchronization process. However the bootstrap method still takes some time as your wallet needs to validate each individual block. 
(source: https://coinguides.org/bitcoin-bootstrap-dat-source-usage/)

# Can I trust this Bootstrap?
Yes you can, the offical BitCanna Announcement was on xx/xx/xxxx on Twitter:
* https://.......
