### Starting Network ###

## Dependencies: 

 * Install mycrypto(https://mycrypto.com/)
 * Install gethtools(https://geth.ethereum.org/downloads/)
 * Download files and add them to geth tools directory
 
## Start Nodes:

* Open First terminal and start first node by running this command:

 ./geth --datadir node1 --unlock "0x63853DBE3bf0bA2e1De3299E0A9AA22C13452D9d" --mine --rpc --allow-insecure-unlock
 
 Enter "spooky" for password
 
* Open Second terminal and start second node by running this command: 

 ./geth --datadir node2 --unlock "881FcE5B85AE3f8d362f66B3109D7217217D547b" --mine --port 30304 --bootnodes "enode://8e42492c5de6bb1397a8e8dbab5cc2d165d4be31a7477b8c35d7ebdc7a7a3c4befbee8656b72bb1e9219c5593151141003ba0d838a4fe91b23f51b5a23f285ec@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock
 
 Enter "spooky" for password
 
## Network Configuration: 

  * Network Name: homework
  * Chain id: 3333
  * Blocktime: Default(15 seconds)
  * Account passwords: "Spooky"
  * Node 1 Key: 0x63853DBE3bf0bA2e1De3299E0A9AA22C13452D9d
  * Node 2 Key: 0x881FcE5B85AE3f8d362f66B3109D7217217D547b
  
## MyCrypto Instructions:

# Adding Network:

  * Open MyCrypto and navigate to 'Change Network' In Bottom Left:
   
   ![Change Network](ChangeNetwork.png)
   
  * Click "Add Custom Node" and Scroll to 'Custom' in the "Network" Column:
  
   ![Custom Network](CustomNetwork.png)
   
  * Fill in settings as shown in image below (Ignore Warnings in image) and press "Save & Use Custom Node":
  
   ![Network Settings](NetworkSettings.png)
   
# Send Transactions:

 * Select the `View & Send` option from the left menu pane, then click `Keystore file`:
 
  ![Keystore File](KeystoreFile.png)
  
 * Select Wallet File and navigate to node1/keystore/ in directory and select the UTC file.
 
  ![Wallet File](WalletFile.png)
  
 * Type "spooky" as password and press unlock:
 
  ![Unlock Wallet](WalletFile.png)
  
 * In the 'Address' box enter node2 (0x881FcE5B85AE3f8d362f66B3109D7217217D547b) and add amount to send
 * Press send and wait to for pop up window, then press 'Check TX status' and confirm logout:
 
 # Congrats your network is working and you just sent your first transaction!