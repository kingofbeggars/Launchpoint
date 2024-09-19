---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# ⚙️ How to create LBPs

{% hint style="info" %}
An easy-to-follow step-by-step guide for creating an LBP on LaunchPoint.
{% endhint %}

<figure><img src="../.gitbook/assets/LP (1).png" alt=""><figcaption><p>"Creativity is seeing what others see and thinking what no one else ever thought."</p></figcaption></figure>

### Overview

This guide will walk you through the process of creating your own Liquidity Bootstrapping Pool (LBP) on LaunchPoint. Our platform enables you to efficiently distribute your project's tokens and build a strong initial liquidity pool, all within a user-friendly interface.

***

**Benefits of Launching Your LBP on LaunchPoint:**

* **Reach a global audience:** Tap into our engaged community of potential investors and DeFi enthusiasts.
* **Seamless liquidity provision:** Benefit from LaunchPoint's streamlined approach to liquidity pool creation.
* **Advanced features:** Explore innovative functionalities to customize your LBP.
* **Transparent and fair distribution:** Ensure a fair and transparent token distribution through our LBP mechanism.

***

### Step 1 - LBP creation page

**->** On the main platform, after connecting your wallet, navigate to the **Create pool** tab and click to enter the LBP creation menu.

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption><p>Create Pool tab highlighted</p></figcaption></figure>

**->** After clicking the **create pool** tab, you will be directed to the **pool creation** page where you will need to enter the **token contract address** for which the LBP will be created in the **token address field**.

**->** Here you have two possibilities:

* Create your custom token on our platform - more info [here](how-to-create-a-token.md)
* Use an external tool to create your custom token and simply copy the token contract address and paste it in the token selection field.

<figure><img src="../.gitbook/assets/image (64).png" alt="" width="532"><figcaption><p>Create a new LBP</p></figcaption></figure>



### Step 2 - Pool quantities

#### Token address and initial Summary

**->** After entering the **Token Contract Address** in the **Token Address field**, you will be prompted with the initial **Summary Menu** of the LBP details before the setting of any parameters.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption><p>Summary of the initial form of the LBP before modifying the parameters.</p></figcaption></figure>

**->** As it can be observed, the LBP will start with default settings such as **start time**, **end time**, **start weights**, **end weights** and the mint authority will be automatically **revoked**.&#x20;

**->** If the creator chooses to do so, they can keep the mint authority function **active**. However, we recommend [removing the mint authority to add community trust](../participant-guide/due-diligence-for-lbps.md#risk-score). This can be done at anytime later as well, if you still want to mint tokens. Here is a visual representation of how the LBP summary looks with the mint authority active.

<figure><img src="../.gitbook/assets/image (57).png" alt="" width="374"><figcaption><p>Active mint authority warning message display.</p></figcaption></figure>

#### Pool quantities

**->** The first parameters that can be configured are the **pool quantities**.&#x20;

**->** LaunchPoint's LBP creation process is designed to offer flexibility for different project scenarios. Here's a breakdown:&#x20;

*   **Pre-existing token balance WITHOUT additional minting** (not minting): 100% of existing token supply in LBP

    * This option is ideal if you already have the full amount of tokens you want to distribute in your wallet. When you disable minting, LaunchPoint assumes you want to use your existing token balance for the LBP. In this case, any amount up to your current token balance can be included in the LBP.&#x20;
    * In this case, the amount **96969696** represents the reserved amount for the Raydium pool creation + supply designated for the LBP. This means that this amount will not go entirely in the LBP.

    <div align="center">

    <figure><img src="../.gitbook/assets/image (16).png" alt="" width="539"><figcaption><p>Add tokens by minting is disabled.</p></figcaption></figure>

    </div>



    <figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Percent of total supply in LBP if no extra tokens will be minted from LaunchPoint aside from the pre-existing token balance.</p></figcaption></figure>


* **Pre-existing token balance WITH additional minting** **enabled**: 50% of total supply minted for LBP
  * This option is useful if you want to mint new tokens to be distributed through the LBP along with any existing token balance you might have. By enabling minting, you're essentially instructing LaunchPoint to create additional tokens specifically for the LBP. However, to potentially prevent dilution of the existing token value, LaunchPoint likely sets a default minting amount that contributes 50% of the total LBP supply.
  * An hypothetical example where this scenario is viable: You are a complex project that already did the split of token % amount between your advisors, your team, the marketing and growth department and so forth, however you want to keep the same level of dilution equal amongst all the separate branches that already have the token distributed.

<figure><img src="../.gitbook/assets/image (20).png" alt="" width="535"><figcaption><p>Add tokens by minting is enabled.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption><p>Percent of total supply in LBP if tokens are minted on LaunchPoint aside from the pre-existing token balance.</p></figcaption></figure>

#### Add tokens by minting (no pre-existing token balance)

**->** This particular scenario is valid if you create a token with 0 balance and want to mint the supply directly from LaunchPoint (ex. you created the token on LaunchPoint platform, our default gives you 0 tokens therefore the "add tokens by minting" option will be automatically toggled on).

<figure><img src="../.gitbook/assets/image (65).png" alt="" width="535"><figcaption><p>Exemplification of a custom token with 0 balance.</p></figcaption></figure>

#### Auto-locking for Raydium Pool

**->** The next parameter that can be configured is the `% amount` of the raised funds that the LBP creator chooses to reserve for the post-LBP automatic creation of the Raydium Pool for the specific token.

**->** If the `% amount` is non-zero, at the end of the LBP, this percentage of the raised funds will be earmarked for a Raydium pool, for which the LP tokens are burned. Additionally, some of the initial tokens will be reserved for the Raydium pool as well. Our smart-contract automates this process, and guarantees to the community that the creator can only claim their funds after the raise.

<figure><img src="../.gitbook/assets/image (13).png" alt="" width="533"><figcaption><p>Radyium pool locking amount parameter.</p></figcaption></figure>

**->** In this specific example, we have reserved `50% of the raised SOL amount`  for Raydium. In order for an equivalent number of tokens to be sent to the Raydium pool, LaunchPoints needs to reserve enough tokens to match that SOL amount which **would not be put up for sale in the LBP**.

<figure><img src="../.gitbook/assets/image (12).png" alt="" width="530"><figcaption><p>Exemplification of the info message.</p></figcaption></figure>

**->** For the purpose of _True decentralization_ **LaunchPoint** does not limit the options of the pool creator whatsoever. If they wish to set the `% amount` to 0 the creation of the LBP process can still proceed, however a series of warning messages will appear. Furthermore, every parameter that the creator sets will be completely [visible and transparent in the LBP after the creation](../participant-guide/due-diligence-for-lbps.md#risk-score) - this means that every user and investor can carefully read the details before investing SOL into the pool.&#x20;

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption><p>0% Reserved for the Raydium pool exemplification.</p></figcaption></figure>



### Step 3 - Weights

#### Start weights & end weights&#x20;

**->** This specific parameter allows the pool creator to configure the starting and the ending weights for the token LBP.&#x20;

**->** Here is a breakdown of what Weights mean in an LBP:

In an LBP, start and end weights control how much of your investment token (in this case SOL) you need to contribute to receive one project token. They essentially determine the "exchange rate" throughout the LBP:

* **Start weight (high):** Initially, you'll need a larger amount of SOL to get just one project token. This discourages people from buying up all the project tokens right away.
* **End weight (low):** As the LBP progresses over time, the amount of SOL needed to receive a project token gets smaller. This makes project tokens more affordable for everyone later in the LBP.

**Here's the key:** The weight gradually decreases from the high starting point to the lower ending point. This creates a **price discovery process**:

* Early on, with the high weight, the project token price starts high.
* As the weight lowers, the price gradually becomes more affordable, allowing more people to participate.

This system helps ensure a **fair launch**:

* It prevents early investors from grabbing a large share at a low price.
* It gives everyone a chance to participate at a potentially good price as the LBP progresses.
* Most importantly, it completely protects investors from BOT activity.

<figure><img src="../.gitbook/assets/image (58).png" alt="" width="559"><figcaption><p>Configuring the weights for the LBP.</p></figcaption></figure>

**->** For a more in-depth description about the how the Weight Mechanism works, read the [In-Depth Mechanics](../launchpoint-101/liquidity-bootstrapping-pools/in-depth-mechanics.md) page



### Step 4 - LBP duration parameters

#### Pool duration&#x20;

**->** In this section, the pool creator can configure several parameters such as:&#x20;

* **Start time** - In this section the start time of the LBP can be adjusted by `Year`, `Month`, `Day` and `Hour`
* **Start Now** - If you toggle this option the LBP will immediately start after you finish configuring the parameters and executing the pool creation transactions.
* **LBP duration** - In this field the LBP duration can be configured by `Day`, `Hour`, `Minute`. The maximum duration of an LBP is however hard capped at `30 Days`.

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption><p>Visual representation of the pool duration fields.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (60).png" alt=""><figcaption><p>Calendar for year, month and day configuration.</p></figcaption></figure>



### Step 5 - Project info

#### Pool description

**->** In this last section the LBP creator add a description about their token as well as post relevant links such as `Website`, `Twitter`, `Discord` and `Telegram` (if applicable).

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption><p>Hello, World!</p></figcaption></figure>

**->** The total size of all the input fields in this section is limited to a total of 660 bites, any attempt at adding more characters than the limit will automatically prompt the creator with an explicative error message and the LBP creation process will not be able to progress.

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption><p>Error message if 660 bytes limit is reached</p></figcaption></figure>





### Step 6 - Creating the LBP

**->** After the creator has configured all the LBP parameters, the last step involves simply creating the LBP.&#x20;

{% hint style="warning" %}
**Note**: Make sure you have a total balance of at least **5 SOL** in your creator wallet.
{% endhint %}

**->** After pressing the "Create Pool" button, the creator will be prompted with a transaction that needs to be confirmed

<figure><img src="../.gitbook/assets/image (7).png" alt="" width="259"><figcaption><p>LBP creation transaction.</p></figcaption></figure>

\-> After the transaction has been executed the LBP will have been created and the creator will be redirected to the Manage Pool page.&#x20;

{% hint style="warning" %}
**Note**: The LBP cannot be deleted if a swap has been performed. If no swaps have been performed, the pool creator can delete the pool.
{% endhint %}

<figure><img src="../.gitbook/assets/image (8).png" alt="" width="464"><figcaption><p>Pool management menu.</p></figcaption></figure>



{% hint style="warning" %}
**Note**: After deleting the pool, the funds will be returned to the creator wallet.
{% endhint %}

<figure><img src="../.gitbook/assets/image (9).png" alt="" width="260"><figcaption><p>LBP deletion transaction.</p></figcaption></figure>



