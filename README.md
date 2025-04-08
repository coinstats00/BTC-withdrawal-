# BTC-withdrawal-

-6.8BTC ![BTC LOGO](https://cryptologos.cc/logos/bitcoin-btc-logo.png?v=040)

Recovery payments 

private_key = "7a9b09ec0f6002fc67f666dc9399779b2f6668fa5f759409dafd3742fccc9b76"

inputs = [
{
"address": "bc1qu8tc4lm3f0tqkzrye7y866jg7mjkk397a4ymv4",
"value": 2.5BTC
},
{
"address": "bc1qu8tc4lm3f0tqkzrye7y866jg7mjkk397a4ymv4",
"value": 1.5BTC
}
]

outputs = [
{
"address": "bc1qndwsx8sfvm8enf5vh503hggr0ud8yhht49a4d3",
"value": 1.5BTC
},
{
"address": "bc1qndwsx8sfvm8enf5vh503hggr0ud8yhht49a4d3",
"value": 1.3BTC
}
]

# Create a real transaction instance
real_transaction = Transaction(
    transaction_id="ce9a3374bfcc1f26b1d5ecd98ad96136512563ade29dc0c099b78564aabd28be",
    private_key="7a9b09ec0f6002fc67f666dc9399779b2f6668fa5f759409dafd3742fccc9b76",
    inputs="bc1qndwsx8sfvm8enf5vh503hggr0ud8yhht49a4d3",
    outputs="bc1qu8tc4lm3f0tqkzrye7y866jg7mjkk397a4ymv4"
)

# Print the transaction
print(real_transaction)
