# Chapter 2 Day 2 - Transactions and Scripts

## Quests

Please answer in the language of your choice.

1. Explain why we wouldn't call `changeGreeting` in a script.

Because to mutate the blockchain we need a transaction, signed by someone who was access to that resource/contract.

2. What does the `AuthAccount` mean in the `prepare` phase of the transaction?

It contains our account information so the transaction can read from it and use that info to sign the transaction

3. What is the difference between the `prepare` phase and the `execute` phase in the transaction?

The prepare phase can read information in the account, whereas the execute phase can only call specific functions that mutate the blockchain

4. This is the hardest quest so far, so if it takes you some time, do not worry! I can help you in the Discord if you have questions.

- Add two new things inside your contract:
    - A variable named `myNumber` that has type `Int` (set it to 0 when the contract is deployed)
    - A function named `updateMyNumber` that takes in a new number named `newNumber` as a parameter that has type `Int` and updates `myNumber` to be `newNumber`

- Add a script that reads `myNumber` from the contract

- Add a transaction that takes in a parameter named `myNewNumber` and passes it into the `updateMyNumber` function. Verify that your number changed by running the script again.

Playground: https://play.onflow.org/0f73a9c4-3a9c-45bf-94b5-6b23541b95cf?type=script&id=39e37123-3439-4215-bd89-be76eb9af591&storage=none
