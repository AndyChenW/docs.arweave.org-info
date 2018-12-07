---
description: >-
  Want to start mining on Arweave? You've come to the right place! Get set up
  with this quick and easy guide, and join our awesome network of ever-growing
  miners.
---

# Mining Guide



## Preparation: Linux 

1. **Install an up-to-date version of** [**Erlang**](https://www.erlang.org/downloads) **\(Erlang/OTP 20+\), git and libssl-dev or equivalent**

   \(usually available from your Linux distribution’s package manager\)

2. **Use git to clone the latest stable release using the following command:**

```
git clone https://github.com/ArweaveTeam/arweave.git arweave && \
cd arweave && git -c advice.detachedHead=false checkout stable
```

Alternatively, you can simply run this [script](https://raw.githubusercontent.com/ArweaveTeam/arweave/master/install.sh) on a fresh Ubuntu installation. Because this script installs dependencies for you it will require your root password, so please make sure you are comfortable with the commands that it will run before execution. You can download and execute the script with this command:

```bash
curl https://raw.githubusercontent.com/ArweaveTeam/arweave/stable/install.sh | bash
```

## Preparation: Other Operating Systems

In order to run the Arweave miner on Mac OS X please execute the following steps:

1. **Install** [**Homebrew**](https://brew.sh/)\*\*\*\*
2. **Run ‘brew install erlang@20’**
3. **Finally, run the following command:** 

```text
git clone https://github.com/ArweaveTeam/arweave.git arweave && \
cd arweave && git -c advice.detachedHead=false checkout stable
```

{% hint style="info" %}
It is also possible to set-up an Arweave mining environment on Windows using the ‘Windows Subsystem for Linux’ or a virtual machine environment
{% endhint %}

## Running the Miner

Now you’re ready to start the mining process by using the following command from the Arweave directory: 

```text
./arweave-server \
                peer 52.56.119.91 peer 34.216.88.202 \
                peer 54.93.54.173 peer 18.130.126.49 \
                peer 13.231.142.3 peer 18.179.119.203 \
                peer 54.159.24.25 peer 54.175.114.204 \
                mine mining_addr YOUR-MINING-ADDRESS
```

{% hint style="warning" %}
Please replace **YOUR-MINING-ADDRESS** with the address of the wallet you would like to credit when you find a block!
{% endhint %}

If you would like to see a log of your miner’s activity, you can run **‘make log’** in the Arweave directory in a different terminal. The miner terminal itself is left clear so that you can interact with the system using the console. 

## Staying up to Date

* Join our [Discord](https://discord.gg/kh9BeEm) server
* Join our mining mailing list

Once you are successfully mining on the Arweave, you will need to stay up to date with new releases. [Join our mailing list](https://mailchi.mp/fa68b561fd82/arweavemining) to receive emails informing you that a new update has been released, along with the steps you need to take to stay up to speed. Updates that require you to perform an action within a certain time period in order to stay in sync with the network will be labeled ‘\[ACTION REQUIRED\]’. Keep an eye out for these messages, and if possible make sure that you add team@arweave.org to your email provider’s trusted senders list!

**We also recommend that you join our** [**Discord server**](https://discord.gg/kh9BeEm) **as this is the hub of our mining and developer communities. Here you will find plenty of community members or team members available to help you out** [👾](https://emojipedia.org/alien-monster/)





