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

# ❓ FAQs for participants

{% hint style="info" %}
A comprehensive guide for navigating LaunchPoint as a LBP participant.
{% endhint %}

<figure><img src="../.gitbook/assets/53.png" alt=""><figcaption><p>“I’m a scientific expert; that means I know nothing about absolutely everything.”</p></figcaption></figure>

***

### <mark style="color:blue;">What is a LBP (Liquidity Bootstrapping Pool) ?</mark>

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

### <mark style="color:blue;">How LaunchPoint LBPs work for you</mark>

* These dynamic pools offer a more interactive experience compared to traditional Dutch auctions. While Dutch auctions start with a high price that gradually decreases, LaunchPoint LBPs allow you to buy in at any point during the process, potentially influencing the price itself.&#x20;
* Increased buying activity can even cause temporary price increases! This creates a fair and engaging marketplace for acquiring new project tokens.

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

### <mark style="color:blue;">What's the best time to buy into an LBP ?</mark>

The ideal time to buy in depends on your personal assessment of a fair price for the token. Understanding weights plays a crucial role in this decision.&#x20;

* For instance, an LBP starting with a 98% Project Token to 2% SOL ratio and ending at 90% SOL to 10% Project Token could experience a significant price drop if there are few buyers. This presents an opportunity to acquire tokens at a lower price.
* On the other hand, an LBP starting at a 75% Project Token to 25% SOL ratio and ending at 25% Project Token to 75% SOL might have a less drastic price decline with fewer new buyers. This results in a more stable pricing curve, potentially offering less of a discount on tokens by the LBP's end.

By understanding weight shifts, you can make informed decisions about when and at what price to participate in a LaunchPoint LBP.

***

### <mark style="color:blue;">Can I provide liquidity in LaunchPoint LBPs ?</mark>

* No, currently, only LBP owners can add and remove liquidity.

***

### <mark style="color:blue;">What is the difference between curated and uncurated LBPs ?</mark>

At LaunchPoint, we prioritize showcasing high-quality projects with our multi-layered curation system. This system analyzes projects seeking to raise liquidity on our platform, ensuring they meet our standards. The projects that pass this rigorous review process are labeled "Curated" within the LBPs for your reference.

However, we understand that not all projects fit neatly into traditional categories. For full transparency, we also allow projects with a more experimental or "degen" nature to launch on LaunchPoint. These projects are labeled "Uncurated" within the LBPs.

Here's a breakdown to help you navigate these distinctions:

**Curated projects:**

* **Thoroughly reviewed:** These projects have undergone a multi-step review process, often involving our internal team and potentially even third-party curators chosen by the project itself.
* **Credibility boost:** While curation doesn't eliminate risk entirely, it adds a layer of reassurance that the project has been vetted.
* **Do your research:** We recommend consulting the curators' reports (if available) to understand the basis for their approval.&#x20;
* **Not risk-free:** Remember, even curated projects involve inherent risks. Always conduct your own research before investing. More info [here](due-diligence-for-lbps.md)

**Uncurated Projects:**

* **Direct launch:** These projects haven't undergone our curation process and have opted to launch directly through LaunchPoint's LBP contracts on the blockchain.
* **Lower visibility:** Uncurated projects are not prominently featured within the LaunchPoint UI to ensure users are aware they haven't been reviewed.
* **Increased caution:** When encountering uncurated projects, LaunchPoint provides additional warnings to highlight the potential risks involved. Proceed with an extra dose of caution and conduct thorough due diligence before investing in an uncurated project.

By understanding these distinctions, you'll be better equipped to make informed decisions about participating in LaunchPoint LBPs. Remember, both curated and uncurated projects carry inherent risks. Always perform your own research before investing.

***

### <mark style="color:blue;">Will I be able to buy and sell tokens during an LBP ?</mark>

Absolutely, you can participate in LaunchPoint LBPs by both buying and selling tokens throughout the process. Our platform fosters a dynamic environment for price discovery, fueled by buy and sell orders from participants like you.

Here's a breakdown of how buying and selling work during LaunchPoint LBPs:

* **Buying tokens:** You can acquire project tokens at any point during the LBP. Remember, the price typically starts high and gradually decreases as the LBP progresses. This allows you to enter the market at a price point that aligns with your investment strategy.
* **Selling tokens (if applicable):** For some LBPs, especially those involving projects with existing token circulation, you might also be able to sell tokens you already own back into the pool. This can add liquidity to the pool and potentially influence the price discovery process.

**Transparency is key:**

LaunchPoint prioritizes transparency throughout the LBP process. This includes providing clear information about whether the project has existing token circulation and if selling back to the pool is an option for participants.

***

### <mark style="color:blue;">Does LaunchPoint charge fees for participating in LBPs ?</mark>

Yes, LaunchPoint has a two-tier fee structure for LBPs:

* **2% Swap fee:** A 2% fee applies to all token swaps that occur during an LBP. This fee helps maintain the platform and ecosystem.
* **3% Raised amount Fee:** Project creators are charged a 3% fee on the total amount of funds raised through their LBP.

***

### <mark style="color:blue;">What risks are involved in participating in LBPs ?</mark>

* **Market volatility:** The cryptocurrency market is inherently volatile. The value of project tokens acquired through LBPs can fluctuate significantly.
* **Impermanent loss:** Investors who provide liquidity early may experience impermanent loss if the token price falls significantly.
* **Complexity:** Understanding how LBPs work can be complex for new investors. However, with enough time and patience even new users can get quickly accustomed to our platform by going through our documentation!

***

### <mark style="color:blue;">How long do LaunchPoint LBPs typically last ?</mark>

* LaunchPoint offers flexibility to project creators when it comes to LBP duration. While the majority of LBPs conclude within a reasonable timeframe, the exact length is determined by the project team themselves. The maximum duration for a LaunchPoint LBP is 30 days. Each LBP's specific timeline will be clearly displayed on its dedicated page, allowing you to plan your participation accordingly.

***

### <mark style="color:blue;">What is slippage and how does it affect my purchase ?</mark>

* Slippage refers to a potential difference between the price you expect to pay for a token and the final price you pay when the transaction is completed. This can occur in LaunchPoint LBPs because token prices adjust dynamically in real-time based on buy and sell orders within the pool.
* It's important to understand that slippage isn't necessarily caused by high market volatility, but rather a characteristic of decentralized trading mechanisms. Slippage can work in your favor or against it, meaning you might receive slightly more or less than the anticipated amount of tokens.

**Managing slippage during LaunchPoint LBPs**

* To manage potential slippage, you can set a "slippage tolerance" level within your transaction. This represents a percentage range you're comfortable with when it comes to price variations. If the actual slippage exceeds your set tolerance, the transaction won't be executed. Therefore, it's crucial to be aware of your slippage tolerance settings and adjust them based on your risk comfort level before participating in a LaunchPoint LBP.

***

### <mark style="color:blue;">What token can I use to participate in a LaunchPoint LBP ?</mark>

* In LaunchPoint LBPs, there's a single collateral token supported for participation: <mark style="color:purple;">**SOL**</mark>. This means you'll need to have SOL in your wallet to be able to buy tokens offered through LaunchPoint LBPs. The specific LBP details will clearly display this requirement, so double-check before you commit to buying.



