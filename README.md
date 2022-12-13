## Build an Image ##

docker build --tag 21204811 .


## Run an image ##

docker run --name 21204811 -p 8090:8080 21204811

## Run the curl command ##

This transfers ETH:

curl --header "Content-Type: application/json" --request POST --data '{"address":"0x1DfFa18c1C2C1dE13177707E582B6d15DC4473D6", "amount":"0.05"}' http://localhost:8090/eth

This transfers token:


curl --header "Content-Type: application/json" --request POST --data '{"address":"0x1DfFa18c1C2C1dE13177707E582B6d15DC4473D6"}' http://localhost:8090/token



