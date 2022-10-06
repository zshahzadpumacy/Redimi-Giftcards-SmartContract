# Redimi-Voucher-SmartContract\

Redimi solution comprises of several modules where each module accomplishes a crucial task. Following is the list of these modules:

## 1. Smart Contracts (SCs)

This module involves development and deploying of smart contracts on Blockchain using Solidity to manage gift cards and coupons. The smart contracts also define security measures to prevent fraudulent transactions by utilizing signatures from multiple parties e.g., customer and retailer. Since each entity participating in this solution requires a Wallet (ethereum), the private keys are used to authorize the transactions on the smart contract. Currently, a separate smart contract exists for management of gift cards and coupons.

### a. SC for Gift Cards

 The smart contract for gift cards is capable of following functionalities:
 
 * Creation of gift cards: When a customer purchases a gift card at the Mall, this transaction takes place on the smart contract where specific information is stored including wallet addresses of customer and mall, purchase and expiry date, amount etc.
 
 * Redemption of gift cards: The gift cards can be redeemed at supported retailers. When a gift card is redeemed, this transaction takes place on the smart contract which also updates the amount available in the gift card. To prevent fraud, signatures from customer and retailer are used to authenticate the transaction.
 
 * Transfer voucher ownership: This functionality allows customers to transfer the gift cards to one another. 
 
 * Transfer voucher amount: Apart of transfering a complete voucher, customers can also transfer partial amounts from one voucher to another. 
 
 * Manage retail partners of the mall: Since gift cards purchased from a mall are only redeemable through supported retailers, this functionality allows adding/removing partner retailers.
 
 ### b. SC for Coupons
 
 The smart contract for coupons is capable of following functionalities:
 
 * Creation of coupons: Malls/retailers can create coupons based on several use cases including targeted coupons i.e. creating coupons for a specific list of customers or creating coupons for all the customers. The coupons can have a certain redeem limitations as well.
 
 * Redemption of coupons: Similar to gift cards, coupons can also be redeemed at the supported retailers where relevant discount is provided to the customer based on the coupon description including discount type, discount value etc. 
 
