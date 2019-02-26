**1. Setup a MasterNode**

**Prerequisite**

 1. Operating System : Ubuntu 16.04 64-bit or higher Should be facing internet directly with public IP & without NAT

 2. Tools: Git, Docker, Docker Compose

 3. Network Ports

Following network ports need to be open for the nodes to communicate.

8545  TCP - RPC <br>   
30303 TCP/UDP - XDC

**How to Setup Masternode ?**

**0. Install Git**

* Check whether git is preinstalled.

    > git --version

If present, output will be something like git version 2.17.1. in this case, go to step a.

* Otherwise follow the below steps.

    1. sudo apt update
    2. sudo apt install git
    3. git --version

* Configure Git.

    1. git config --global user.name "Your Name"
    2. git config --global user.email "youremail@domain.com"

**a. Clone repository**

Run the following commands on your terminal.

    1. git clone [https://github.com/XinFinOrg/XinFin-Node.git](https://github.com/XinFinOrg/XinFin-Node.git)
    2. cd XinFin-Node

The git clone command will create a new folder XinFin-Node. cd XinFin-Node command changes the current directory to XinFin-Node

**b. Install docker & docker-compose**

       sudo ./install\_docker.sh

The above command will install docker and docker-compose for you.

**c. Update .env file with details**

* Copy a env.example file from XinFin-Node directory and name it as a .en
* Open .env file and edit values for following

     1. INSTANCE_NAME : A Display name of your masternode
     2. CONTACT_DETAILS : Your Email ID

![overview](/assets/xinfin-node.png)

![overview](/assets/masternode-.env.png)


**d. Start your Node**

        sudo docker-compose -f docker-services.yml up -d

This will start a Masternode and connect to a XinFin Testnet.

You should be able to see your node listed on this page: [XinFin Network](https://www.xinfin.network) (Make sure, you are connected to XinFin Testnet. If not, switch to Tesnet on top right corner)

Your coinbase address can be found in xdcchain/coinbase.txt file.

![overview](/assets/masternode-listing.png)

**2. Stake XDC**

  **Create XDC Wallet**

      > Visit http://xinfin.network/#webWallet and Click on create a new wallet.
      > you can create use a web wallet or download eWallet app from Google Play Store.
      > Create an account
      > Store your private key at a safe place (Hardware wallet is recommended)

![overview](/assets/xinfin_wallet.png)


   **Buy XDC**

     > get your free XDC to use on XinFin Testnet
     > Visit XinFin TestNet Faucet http://xinfin.network/#getTestXDC.
     > Add your wallet address created in step 2.b and request XDC

![overview](/assets/masternode-faucet.png)

   **Upload Kyc**

    > Visit http://xinfin.network/#masternode
    > Upload a notarized kyc

![overview](/assets/masternode-node.png)