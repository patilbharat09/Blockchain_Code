## Compiling the ECR20.sol file ##

Compile the code present in ERC20.sol file

## Deploying the code ##

Deploy the code, after successful deployment, the contract would be created in Etherscan

## Etherscan ##

View the transaction on Etherscan, then use the Contract Address to Verify and Publish the Contract. After the contract is Verified and Published, copy the ABI key and update the python files where it has been called.

## Importing the tokens in MetaMask ##

Use the Contract Address to import the tokens into MetaMask account. A million Shibi tokens would be imported with the unique name (Here it is "SHB_04811").

## Update the .env file ##
Update the following things in the .env file:
CONTRACT_ADDRESS
OWNER_ADDRESS
SUPER_SECRET_PRIVATE_KEY

## Build an Image ##

docker build --tag 21204811 .

## Run an image ##

docker run --name 21204811 -p 8090:8080 21204811

## Run the curl command to transfer the token ##

curl --header "Content-Type: application/json" --request POST --data '{"address":"0x1DfFa18c1C2C1dE13177707E582B6d15DC4473D6"}' http://localhost:8090/token

A token would be transferred from your account to the account mentioned in the curl command (0x1DfFa18c1C2C1dE13177707E582B6d15DC4473D6).
