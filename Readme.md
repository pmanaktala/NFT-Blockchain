
| Name      | Email Id | Github Link |
| ----------- | ----------- | --------- |
| Parth Manaktala      | manap01@pfw.edu       | https://github.com/pmanaktala/NFT-Blockchain |

# Setting project on local
## Step 1 : Setting Morlais Server on Local
Since moralis v2 has no longer support for web3 server on local, we will have to setup a web3 moralis server on local. To do so, I followed the official documentation. Link -> [How to Set Up a Self-Hosted Web3 Server](https://moralis.io/how-to-set-up-a-self-hosted-web3-server/)

## Step 2 : Cloning the repository
Cloning the repository given in the video

## Step 3 :  Setting up variables
There are two variables that needs to be set in the `Logic.js` file to configure Moralis

    Moralis.initialize("123"); // Application id from moralis.io
    Moralis.serverURL = "http://127.0.0.1:1337/server"; //Server url from moralis.io
    
Over here the moralis app id is the id we set in the local server, and serverURL is the path to local server.

## Step 4 : Installing the dependencies and running the build.

Running the following command in the code directory to install the dependicies and building the code.

    npm install
    npm run build
    
## Step 5 : Running the application and logging in to Morlais

We run the application using the `npn run dev` command and filling in the form and clicking on `Connect Metamask` button.

> While logging in, we are getting an due to mismatch of moralis version (V2) and the Javascript SDK (V1) in the python applicaiton. Hence, was not able to proceed further.