---
description: Frequently asked questions.
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

# ❓ FAQ for creators

_This page will get constant updates as time advances and the project evolves._

***

<figure><img src="../.gitbook/assets/IMG08 (1).png" alt=""><figcaption><p>"If you have knowledge, let others light their candles in it."</p></figcaption></figure>

***

### <mark style="color:blue;">What is an LBP (Liquidity Bootstrapping Pool) ?</mark>

An LBP is a smart contract used on decentralized exchanges (DEXs) to create initial liquidity for new cryptocurrency projects. It helps ensure there are buyers and sellers readily available when a new token launches.

#### LBP components

* **Smart contract:** The core of an LBP is a smart contract deployed on a decentralized exchange (DEX). This contract defines the rules of the pool, including the initial price, price curve, and fundraising duration.
* **Tokens:** The LBP involves two types of tokens:
  * **Project token:** This is the new token being launched by the project team.
  * **Base token:** This is an established cryptocurrency, often a stablecoin like USDC, used to purchase the project token.
* **Liquidity pool:** The LBP creates a liquidity pool where project tokens and base tokens are deposited. This pool facilitates trading of the project token upon launch.

#### LBP functionalities

* **Price discovery:** Through an automated price curve, the LBP dynamically sets the price of the project token based on demand. This price typically starts high and gradually decreases over a predetermined period.
* **Fundraising:** Investors can purchase project tokens from the liquidity pool using the base token. These purchases contribute to the project's fundraising goals.
* **Fair distribution:** The decreasing price curve incentivizes early participation and discourages bots or large investors from manipulating the price. This aims to achieve a fairer distribution of tokens among a wider range of participants.
* **Automated liquidity provision:** As investors buy project tokens, they also contribute to the liquidity pool. This helps create a readily available market for the project token after the LBP concludes.

#### Additional information

* LBPs are used on decentralized exchanges (DEXs).
* They are an alternative to traditional Initial Coin Offerings (ICOs).
* LBPs offer benefits like fair price discovery, reduced volatility, and decentralized fundraising.
* However, investors should be aware of potential drawbacks like impermanent loss (for liquidity providers) and complexity in understanding how LBPs work.

***

### <mark style="color:blue;">How do LBPs work ?</mark>

* An LBP is a pool where the price starts high and decreases over time depending on buy pressure, which allows more individuals to enter at a fair price during this early stage. This creates an incentive for early participation and helps raise funds for the project.

***

### <mark style="color:blue;">What are the benefits of using an LBP ?</mark>

* **Fair price discovery:** LBPs can help discover a fair market price for a new token through organic buying and selling.
* **Reduced volatility:** By creating initial liquidity, LBPs can help reduce price volatility for the new token.
* **Decentralized fundraising:** LBPs enable projects to raise funds in a decentralized manner, without relying on traditional venture capitalists.

***

### <mark style="color:blue;">What makes this more fair than other tokens ?</mark>

* We leverage weighted pools for initial liquidity bootstrapping in order to ensure a fair distribution mechanism.&#x20;

***

### <mark style="color:blue;">Why is this important ?</mark>

* If a token launches on a traditional liquidity pool on DEX, supply is at risk of uneven distribution because snipers and MEV bots race to buy first a big chunk of tokens, then capitalize by dumping tokens on normal users who want to buy. There's no accessible way to compete with this.
* However, taking part in a LBP guarantees protection for initial buyers as by design snipers can't win if they rush to buy. This way, tokens get distributed to the actual community at a fair rate.
* After the end of a LBP, listing the token on a traditional DEX would allow price discovery having a fair distribution of early of tokens for early buyers.
* Price discovery can also happen during the LBP if demand is too high, but an extreme price increase would be priced in terms of market cap while still having a fair supply distribution.

***

### <mark style="color:blue;">Why choose LaunchPoint LBPs over batch auctions ?</mark>

* Unlike batch auctions, where token allocation is based on pre-determined contributions (potentially favoring large investors), LaunchPoint LBPs offer a more equitable landscape.&#x20;
* The dynamic pricing system starts high and gradually decreases, allowing you to enter the market at a comfortable price point. This approach aims for a fairer distribution of tokens among a wider range of participants like yourself.

***

### <mark style="color:blue;">What do weights mean in an LBP ?</mark>

Weights represent the relative value of the project token compared to another asset (often a stablecoin like USDC) within the pool. These weights change over time, impacting the token price:

* **High starting weight:** Imagine a heavier token side on a scale. Initially, you'll need more SOL to acquire a single project token.
* **Weight gradually lowers:** As the LBP progresses, the project token side becomes lighter on the scale. This means you'll need less SOL to buy a project token, making them more affordable over time.

Understanding how weights work equips you to develop a participation strategy and choose the best entry point for you in a LaunchPoint LBP.

***

### <mark style="color:blue;">What should the start and end weights be for my LBP ?</mark>&#x20;

Choosing the start and end weights for your LaunchPoint LBP is an important decision that depends on two factors:

* **Number of tokens you want to distribute:** How many of your project's tokens do you intend to sell through the LBP?
* **Your project's valuation:** What price do you believe your tokens are worth?

Here's a general recommendation to get you started:

* **Start weight:** 99/1

This high initial weighting discourages bots from manipulating the price early in the LBP and sets a strong starting price for your tokens.

* **End weight:** 40/60 (recommended) or up to 50/50

A lower ending weight like 40/60 allows for wider distribution of your tokens, potentially raising more funds. As the weight changes and the token price goes down, more buyers may be incentivized to participate. But if distributing tokens is less of a priority, LBPs with a 50/50 end weight can also be successful. **We recommend avoiding ending weights above 50/49.**

**Rule of thumb for token sales:**

Based on observations, there's a general rule of thumb regarding the percentage of tokens sold in an LBP: it's usually the opposite of the ending weight. For instance:

* **Start at 99/1, end at 10/90:** Expect to sell around 90% of your tokens.
* **End at 20/80:** You might sell roughly 80% of your tokens.
* **End at 75/25:** You'd likely sell around 25% of your tokens.

**Important note:** This is just a rule of thumb, not a guaranteed outcome. The actual percentage of tokens sold can be influenced by various factors, including market conditions and how participants behave during the LBP. It's crucial to closely monitor your LBP and make adjustments based on real-time data and results.

***

### <mark style="color:blue;">How much initial liquidity should I put up for my LBP ?</mark>

#### How much initial liquidity should I put up for my LBP?

The amount of initial liquidity you provide (the tokens paired with your LBP tokens) is a strategic choice for your team. Here are some factors to consider:

* **Project valuation:** How much do you believe your project's tokens are worth?
* **Target LBP raise:** How much do you aim to raise through the LBP?

LaunchPoint currently only allows using SOL to buy LBP tokens.

**Liquidity considerations:**

While the exact amount of liquidity will vary depending on your project, our experience shows that it's possible to generate sufficient liquidity even with a starting amount of just 1 SOL, assuming there's demand for your token. Of course, providing a higher amount (around $30k is a common starting point for many LBPs) can also lead to strong results.

**Remember:** Closely monitor your LBP's performance and adjust the liquidity pool as needed based on real-time data and market conditions.

***

### <mark style="color:blue;">What are LaunchPoint's platform fees ?</mark>

LaunchPoint has a transparent fee structure to ensure a sustainable platform while offering value to creators. Here's a breakdown of our fees:

* **LaunchPoint fee:** LaunchPoint charges a **3% fee on the total amount raised during your LBP**. This means 3% of the final amount of SOL collected from participants will be used to support platform development and maintenance.
* **Trading fee:** A 2% swap fee is applied to each trade that occurs during your LBP. This fee helps maintain liquidity within the pool, ultimately benefiting your project.

***

### <mark style="color:blue;">What is the difference between curated and uncurated LBPs ?</mark>

At LaunchPoint, we prioritize showcasing high-quality projects with our multi-layered curation system. This system analyzes projects seeking to raise liquidity on our platform, ensuring they meet our standards. The projects that pass this rigorous review process are labeled "Curated" within the LBPs for your reference.

However, we understand that not all projects fit neatly into traditional categories. For full transparency, we also allow projects with a more experimental or "degen" nature to launch on LaunchPoint. These projects are labeled "Uncurated" within the LBPs.

Here's a breakdown to help you navigate these distinctions:

**Curated projects:**

* **Thoroughly reviewed:** These projects have undergone a multi-step review process, often involving our internal team and potentially even third-party curators chosen by the project itself.
* **Credibility boost:** While curation doesn't eliminate risk entirely, it adds a layer of reassurance that the project has been vetted.
* **Do Your research:** We recommend consulting the curators' reports (if available) to understand the basis for their approval.&#x20;
* **Not risk-free:** Remember, even curated projects involve inherent risks. Always conduct your own research before investing. More info [here](../participant-guide/due-diligence-for-lbps.md)

***

### <mark style="color:blue;">When are tokens distributed to participants in an LBP ?</mark>

LaunchPoint ensures a smooth token distribution process for your LBP participants. Here's what they can expect:

* **Automatic allocation:** Tokens are automatically credited to the participant's wallet **immediately after a successful purchase during the LBP**. This means participants don't need to wait until the LBP concludes to receive their tokens.
* **Wallet visibility:** While tokens are automatically allocated, they might not be immediately visible in the participant's wallet interface. In some cases, participants may need to add the token address manually to their wallet to view their holdings.

**For more information:**

* Refer to our guide on adding custom tokens to popular wallets.
* If you have any further questions about token distribution, feel free to reach out to our LaunchPoint support team.

***

### <mark style="color:blue;">Are there hard caps or wallet limits for LBPs on LaunchPoint ?</mark>

**Hard caps:**

LaunchPoint currently does not enforce a hard cap on the total amount of funds that can be raised during your LBP. This allows for maximum flexibility in your fundraising strategy. However, it's important to consider the potential impact on your token price and distribution if there's no limit set.

**Wallet limits:**

LaunchPoint also doesn't impose any wallet limits on participants in your LBP. This means anyone can contribute any amount of SOL within the technical limitations of the Solana blockchain.

**Important considerations:**

* While there are no hard caps or wallet limits, you can still influence the distribution of your tokens through strategic weight settings in your LBP configuration. Refer to the "What should the start and end weights be?" FAQ for more information.
* An unlimited contribution environment can lead to a situation where a single participant acquires a significant portion of your tokens. Consider if this aligns with your project's goals for decentralization and community distribution.

**We recommend carefully evaluating your project's needs and setting appropriate weight settings to achieve your desired token distribution.**

***

### <mark style="color:blue;">Where can I find technical support ?</mark>

LaunchPoint prioritizes providing excellent technical support to our creators. Here's how you can get help:

* **Join our discord channel:** Our active Discord community is a great place to connect with other creators and get real-time assistance. You can find the invite link on our website.
* **Open a support ticket:** Within the Discord channel, you'll find dedicated channels for opening support tickets. Our technical support team will be happy to address your specific questions and troubleshoot any issues you encounter.

**We recommend joining our Discord community to stay updated on the latest platform developments and connect with a network of helpful users.**

***

### <mark style="color:blue;">Can I change the weights during a live LBP ?</mark>

**No, unfortunately, adjusting token weights during an active LBP is not allowed on LaunchPoint.** This is because changing weights mid-LBP could disrupt the price discovery process and negatively impact the overall fairness and efficiency of the fundraising event.

**It's crucial to finalize your start and end weights before initiating your LBP.** We recommend utilizing the LaunchPoint Creation Wizard's preview tool to experiment with different weight settings and find the optimal configuration for your project's goals.





