# Mzansi Web3 Bootcamp Training

## Important resources 📌

- **Mzansi Web3 Bootcamp Dashboard**: [https://www.motokobootcamp.com/]( https://cgjsm-vqaaa-aaaal-qdhma-cai.icp0.io/) (Click on **Login** to access)


### Homework guides 📜

For each of the 10 days of the training, you will find a dedicated daily guide. This guide contains:

1. **Tasks for the Day (✅)**: These are the tasks you'll need to tick off to wrap up the day.
2. **Lectures to Watch (🍿)**: A mix of videos for you to watch. Some are pre-recorded, and for others, you'll need to check the Motoko Bootcamp Calendar for live sessions.
3. **Helpful Resources (📚)**: Here, you'll find links and resources to help you with the day's project.
4. **Concepts Covered (🧠)**: A list of all the concepts we'll go over each day. It's good to skim through this at the start and end of your day to keep track.
5. **Motoko Fact of the Day (💊)**: A quick, interesting, and fun fact about Motoko, Motoko Bootcamp, or the ICP ecosystem.
6. **Meme of the Day (🙈)**: Enjoy some fun memes made by past Motoko Bootcamp grads.

---

Here are the 5 daily guides:

- [Homework 1.](https://github.com/mzansiweb3-icp-hub/mw3_bootcamp/tree/main/homeworks/homework_1)
- [Homework 2.](https://github.com/mzansiweb3-icp-hub/mw3_bootcamp/tree/main/homeworks/homework_2)
- [Homework 3.](https://github.com/mzansiweb3-icp-hub/mw3_bootcamp/tree/main/homeworks/homework_3)
- [Homework 4.](https://github.com/mzansiweb3-icp-hub/mw3_bootcamp/tree/main/homeworks/homework_4)
- [Homework 5.](https://github.com/mzansiweb3-icp-hub/mw3_bootcamp/tree/main/homeworks/homework_5)

### Daily projects ⭐️

During each of the 10 days of training, you'll get to work on a project. You'll need to build it and then submit it on the Mzansi Web3 Bootcamp dashboard. Each project is set up in a similar way:

- **Story (💭) - a quick background story about why this project matters.**
- **Mission (🎯) - a high level explanation of what you’ll need to build today.**
- **Tasks (✏️) - a list of tasks to help you achieve your mission.**
- **Interface (📺) - This is the specific interface your canister should match. Stick to it closely to get your project approved. Remember, even tiny details (like whether a letter is uppercase or not in a function’s name) can make a difference.**

### Start to code 🧑‍💻

For each training day, navigate to the designated folder. For example, on day 1, follow this path:

### Deploy and submit ✅

It’s important to understand that you can deploy your project on 3 different locations:

- **Locally (on your own computer - free)**
  This would be the case if you start a local replica (i.e., a local instance of the Internet Computer running on your machine). This is completely free and used by developers to test their projects. To deploy locally:

  1. **Start a local replica**
     ```jsx
     dfx start --clean
     ```
  2. **Deploy locally**
     ```jsx
     dfx deploy <NAME_OF_THE_CANISTER_TO_DEPLOY>
     ```
  3. **For instance, for the canister of project 1**
     ```jsx
     dfx deploy project_1
     ```
     **⚠️ While deploying projects locally is useful for testing, you won't be able to submit these projects to the Motoko Bootcamp Dashboard. This limitation exists because the dashboard operates on the Internet Computer's main network (mainnet) and is not designed to connect with or recognize projects running on your local replica.**

- **On the Playground (free)**
  The Playground is a special part of the Internet Computer mainnet. It’s a place where developers can develop canisters for free and make them accessible to other canisters on the Internet Computer but it comes with strict limitations:

  - Cycle transfer instructions are silently ignored by the playground (otherwise you’d be able to steal cycles…)
  - Wasm files can't be gzipped.
  - Wasm files will be analyzed to remove any potentially expensive/malicious operations.
  - Canisters can use at most 1GB of memory.
  - Canisters can call the management canister to manage itself without being the controller.
  - Deployed canisters expire after 20 minutes
    The playground is used by the [Motoko Playground](https://m7sm4-2iaaa-aaaab-qabra-cai.raw.ic0.app/) when deploying canisters, but we can also use it with `dfx`. To deploy on the playgound:
    ```jsx
    dfx deploy --playground <NAME_OF_THE_CANISTER_TO_DEPLOY>
    ```
    **💡 Projects that are deployed on the playground can be submitted to the Motoko Bootcamp Dashboard. This is because the playground, despite being a separate section, is still integrated with the Internet Computer. For the entire training period we recommend that you use the playground.**

- **On the Internet Computer (paid)**
  When you deploy an application on the Internet Computer for actual use, it involves some costs. First, there's a fee for setting up a canister, which is roughly $1. Additionally, you need to consider the expense of the cycles required to power your canister. These costs are necessary for deploying a live, functioning application on the Internet Computer.
  1. Setup your identity and get your hands on cycles. You can either pay for it by burning ICPs or receive 10$ worth of cycles if it’s your first time. [Follow this tutorial to receive 10$ worth of cycles.](https://internetcomputer.org/docs/current/developer-docs/setup/cycles/cycles-faucet)
  2. Deploy on the Internet Computer using `dfx`
     ```jsx
     dfx deploy --network ic <NAME_OF_THE_CANISTER_TO_DEPLOY>
     ```
     ⚠️ **If you're working with an online IDE like GitPod, we strongly recommend not deploying directly on the Internet Computer. The reason is that your unique identity gets stored in your online workspace. If you delete this workspace or lose access to it for any reason, you will also lose your identity. Losing your identity means losing control over your canister. To deploy on the Internet Computer, it's safer to set up your environment on your local machine. This will be a necessary requirement for graduation but as stated before, it’s not a requirement for the training, you can use the playground.**

After deploying your project, make sure to record your Canister ID.

![Screenshot 2024-01-03 at 11.09.17.png](./assets/README/readme_3.png)

Then, log in to the Motoko Bootcamp Dashboard, section **Submit,** Level corresponding to the project you are working on and paste the **Canister ID**. Click on **Submit**. Within 10-20 seconds, you should receive a message confirming the submission or indicating an error.

![Screenshot 2024-01-03 at 11.10.24.png](./assets/README/readme_4.png)

If your submission is correct, you can move on to the next project. If you are facing an issue, it’s time to rework your code!

## **Joining a team at Motoko Bootcamp (recommended)** 🤝

[COMING SOON]

## **What’s next?** 🎓

You’ve completed your training? It’s time to prove your skills and graduate. [Click here to continue.](https://github.com/motoko-bootcamp/dao-adventure-graduation)

## **Credits** 🙏

An initiative powered and 100% supported by [Code & State](https://www.codeandstate.com/) - the leading Web3 venture studio for the Internet Computer.
