# Info
This repository is a fork from https://github.com/ton-community/tsc4 \
I solved 4 tasks out of 5 (only task3 left) and won 82 toncoins. My answers are available in contracts folder.
contest page: https://docs.ton.org/develop/func/overview#contests

# 🏆 Welcome to the TON Smart Challenge #4
### by TON Foundation

## 📝 Tasks

1. [task1](/contracts/1.fc) - Find branch of the cell tree
2. [task2](/contracts/2.fc) - Matrix multiplier
3. [task3](/contracts/3.fc) - Find and replace binary substring 
4. [task4](/contracts/4.fc) - Caesar Cipher
5. [task5](/contracts/5.fc) - Fibonacci sequence

Each of the tasks has two parts:

- 📋 A comment with a description of what the smart contract should do.
- 💻 The code of the smart contract with one or more functions marked as `testable`.

The goal of the contestants is to provide a code that matches the description.
Each task may give the contestant either 0 or 5 to 6 score points: 5 for all tests passed plus "gas-score" from 0 to 1 (0 for "infinite" gas consumption, 1 for 0 gas consumption, dependence is inverse exponent).
Each TVM execution is limited to 100,000,000 (hundred million) gas units.
This limit is high enough that it only rules out infinite loops. Any practical solution, regardless of how (un)optimized it is, will fit.

We ask participants not to change the signature (number, order, and types of arguments and result) of `testable` functions for us to be able to evaluate their submission.

## 📅 Solution submission guide and terms

1. **Registration Process**: Before you begin, make sure to go through the registration process via the [@toncontest_bot](https://t.me/toncontest_bot). Your solutions will not be accepted if you are not properly registered.

2. **Create a Private GitHub Repository**: Clone this repository and set it as your own private GitHub repo. Ensuring the visibility configs are set to "private" is crucial to safeguarding your solution.

3. **Set Your Token**: Utilize the `token` provided to you during registration in Telegram bot and set it as a secret variable called USER_TOKEN in your private repository. You can learn more about setting secret variables in the [official GitHub documentation](https://docs.github.com/en/codespaces/managing-codespaces-for-your-organization/managing-encrypted-secrets-for-your-repository-and-organization-for-github-codespaces#adding-secrets-for-a-repository).

4. **Submit Your Solution**: When you are ready to submit your solution, simply push your code into your private repository. The code will be sent to the task review server, and GitHub actions will display the status of your submission.

5. **Solution Evaluation**: If at least one of your solutions works well, your submission will be counted. Feel free to push solutions for more tasks; GitHub actions will run your code against tests and count successful submissions.

6. **Check Your Points**: To check your solution points, review the logs of the GitHub action for your latest commit. Additionally, you can find your solution points in the menu button inside of the Telegram bot.

Best of luck with your submissions!

If for some reason you are not comfortable using the Blueprint environment to write tests for contracts, you can create your own repository. The most important thing is that all your func files with solutions should be in the /contracts folder and named taskN.fc

## 🏆 Prize distribution

Winners of the contest will receive prizes nominated in TON, the native cryptocurrency of the TON blockchain, which is also used as a resource for contract execution.

**The prize distribution will be divided among 3 groups of participants, each receiving 10,000 TON:**

1. The first group will consist of the top 15% of challengers.
2. The second group will consist of 30% of average participants.
3. The third group will consist of the remaining 55% of the contestants.

Participants will be scored based on the following system: each solved problem earns 5 points, and there will be an additional optimization score ranging from 0 to 1 point (where 0 represents an infinite amount of gas spent on the problem, and 1 represents 0 gas spent).

## 📚 Getting Started with TON

For those new to TON development, begin with:

- [Developers Portal](https://ton.org/dev?filterBy=developSmartContract)
- [TON Documentation](https://docs.ton.org)
- [Awesome TON Resources](https://github.com/ton-community/awesome-ton)

Dive deeper into TON with these essential reads:
- [Understanding TON Concepts](https://docs.ton.org/learn/introduction)
- [Writing Smart Contracts](https://docs.ton.org/develop/smart-contracts/)
- [Introduction to FunC](https://docs.ton.org/develop/func/overview)

For pre-built smart contract examples, visit [this section](https://docs.ton.org/develop/smart-contracts/examples).

Stay updated and join discussions on TON Developer Chats:
- English: [@tondev_eng](https://t.me/tondev_eng)
- Chinese: [@tondev_zh](https://t.me/tondev)
- Russian: [@tondev](https://t.me/tondev)

For FunC learners, join the discussion at [@ton_learn](https://t.me/ton_learn).

## 🛠️ Tools for Compilation and Testing

While we recommend [blueprint](https://github.com/ton-org/blueprint) for working with FunC contracts, [toncli](https://ton.org/docs/develop/smart-contracts/testing/toncli) is also a viable option for compiling and local testing.

### Blueprint

Run the following in the terminal to create a new project and choose "A simple counter contract" as an example:

```console
npm create ton@latest
```

Read more about writing tests [here](https://github.com/ton-org/sandbox#writing-tests).

### FunC syntax highlight

For a more streamlined coding experience, consider using [IDE plugins](https://docs.ton.org/develop/smart-contracts/environment/ide-plugins) for syntax highlighting.



