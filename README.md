# transaction.py
from bitcoinlib.wallets import Wallet

# Recovery payments
class Transaction:
    def __init__(self, transaction_id, private_key, inputs, outputs):
        self.transaction_id = transaction_id
        self.private_key = private_key
        self.inputs = inputs
        self.outputs = outputs

    def __repr__(self):
        return f"Transaction ID: {self.transaction_id}\n" \
               f"Inputs: {self.inputs}\n" \
               f"Outputs: {self.outputs}"

# Create a real transaction instance
real_transaction = Transaction( 
    transaction_id="ce9a3374bfcc1f26b1d5ecd98ad96136512563ade29dc0c099b78564aabd28be",
    private_key="7a9b09ec0f6002fc67f666dc9399779b2f6668fa5f759409dafd3742fccc9b76",
    inputs=[
        {"address": "bc1qu8tc4lm3f0tqkzrye7y866jg7mjkk397a4ymv4", "value": 2.5},
        {"address": "bc1qu8tc4lm3f0tqkzrye7y866jg7mjkk397a4ymv4", "value": 1.5}
    ],
    outputs=[
        {"address": "bc1qndwsx8sfvm8enf5vh503hggr0ud8yhht49a4d3", "value": 1.5},
        {"address": "bc1qndwsx8sfvm8enf5vh503hggr0ud8yhht49a4d3", "value": 1.3}
    ]
)

# Print the transaction
print(real_transaction)