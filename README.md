# Bootstrap
Bootstrap.dat is a file that contains the copy of blockchain from genesis block to a certain point of time. This compressed Bootstrap.dat file is used to speed up the initial blockchain download times

# Instructions
* 1.Download from github: https://github.com/BitCannaCommunity/Bootstrap/releases/download/0_300K/bootstrap300k.zip
* 2.Unzip.
* 3.Close your BitCanna node
* 4.Copy the bootstrap.dat file in the "\user\AppData\Roaming\BCNA" folder,  NOT in the "\user\AppData\Roaming\BCNA\blocks" folder.
* 5.Run your BitCanna node again, it should start 'syncing from disk'
