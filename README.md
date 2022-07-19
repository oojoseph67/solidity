1. when using the freeMint.sol/freeMintCondition.sol it is important to note that it is a contract with a hidden data option,
   once minting is done and you are ready to reveal go to the contract on etherscan and change the uriPrefix to the right metadata
   which will be : ipfs://(metadata)/ and write it after that is done you can now set the revealed function to be true................ Also before minting change the paused state to false

2. How the IPFS works:
    - first upload your images to an ipfs cloud
    - copy the ipfs address from the images folder and update the metadata file 
    - update the uri in your smart contract with the .json ipfs (either hidden or public)
    - when you deploy your contract with remix always copy your constructor abi
    
    URI structure = ipfs://(ipfs data)/