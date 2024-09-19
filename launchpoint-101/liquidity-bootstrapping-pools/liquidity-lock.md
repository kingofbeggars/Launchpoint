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

# 🟣 Liquidity lock

{% hint style="info" %}
The importance of the auto-locking mechanic.
{% endhint %}

### Why auto-liquidity lock matters for Raydium pool reserves in LaunchPoint LBPs

The auto-liquidity lock plays a crucial role in ensuring a stable and healthy environment for your token after the LBP concludes.&#x20;

***

**Understanding Raydium pool reserve:**

* When creating an LBP on LaunchPoint, you have the option to allocate a percentage of the raised SOL towards a reserve for the Raydium pool.
* This reserve is essentially a pool of tokens and SOL used to facilitate trading on Raydium after the LBP.
* A well-funded reserve helps maintain liquidity for your token on Raydium, allowing for smoother buying and selling activities.

**The challenge of manual locking:**

* Traditionally, managing liquidity reserves involved manually locking tokens and SOL after the LBP.
* This process could be time-consuming and prone to human error.
* Additionally, there's a risk of delaying the creation of the Raydium pool if the locking process isn't completed promptly.

**Benefits of auto-liquidity lock:**

* LaunchPoint's auto-liquidity lock feature streamlines this process by automatically locking the configured reserve percentage of raised SOL and a corresponding amount of tokens at the conclusion of the LBP.
* This ensures a swift and reliable transition from the LBP to a functional Raydium pool with immediate liquidity.

**Importance in maintaining trust:**

* An auto-locked reserve demonstrates your commitment to providing long-term liquidity for your token on Raydium.
* This can be crucial for building trust with potential buyers during the LBP.
* Knowing that a dedicated reserve exists to facilitate future trading can incentivize participation and potentially lead to a more successful LBP.

**Additional considerations:**

* The auto-liquidity lock typically defines a lock-up period for the reserve, preventing immediate withdrawal. This period helps maintain a stable pool for a predetermined timeframe.
* While LaunchPoint offers auto-locking, it's still essential to understand the specific lock-up duration associated with the reserve to ensure it aligns with your project's goals.



### Understanding final LBP price on LaunchPoint with Raydium pool reserve

This section explains the formula used to calculate the final price of your token after a LaunchPoint Liquidity Bootstrapping Pool (LBP) with a reserve allocation for the Raydium pool.

**Step-by-step breakdown:**

The formula looks like this:

`Total token amount (sold or unsold) / total raised amount (SOL) = Final LBP Price`

`97% represents the raise amount minus our platform raise fee which is 3% and from this final percent x% SOL (our standard is 30% but this value is configurable) that is reserved goes to the Raydium pool.`

Here's a breakdown of each variable and its significance:

1. **Total token amount (sold or unsold):**
   * This refers to the total number of tokens you initially allocated to the LBP, regardless of whether they were all purchased or not.
   * For example, if you set your LBP to distribute 100 million tokens, this value would be 100 million.
2. **Total raised amount (SOL):**
   * This represents the total amount of SOL collected during the LBP.
   * In simpler terms, this is the sum of all the SOL contributions from participants who bought your tokens throughout the LBP.
3. **Final LBP price:**
   * This is the final price per token at the end of the LBP.
   * The formula considers the total token supply, the amount of SOL raised, platform fees, and the reserve allocation for the Raydium pool to arrive at this price.
4. **97%:**
   * This represents the portion of the total raised SOL amount that remains after the LaunchPoint platform fee is deducted.
   * LaunchPoint charges a platform fee of 3% from the total raised SOL.
   * So, 97% signifies 100% (total raised amount) minus the platform fee 3%.
5. **x% (configurable Raydium pool reserve):**
   * This placeholder represents the actual percentage of the raised SOL amount that gets reserved for the Raydium pool.
   * You can configure this percentage in the LaunchPoint pool creation menu. It can be different from the standard 30% mentioned here.
   * This percentage essentially determines how much value from the LBP, represented by SOL, will be used to create liquidity for the Raydium pool.

**Configurable reserve and community trust:**

It's important to note that LaunchPoint allows you to configure the Raydium pool reserve percentage (x%) during pool creation. While a standard 30% might be suggested, you have the flexibility to adjust it.

* Setting the reserve percentage too low (significantly below the standard 30%) could negatively impact the perception of your token by the buyer community. A lower reserve might imply a lack of commitment to long-term liquidity on Raydium, potentially discouraging participation in the LBP.

**In conclusion:**

The auto-liquidity lock in LaunchPoint LBPs with Raydium pool reserves simplifies the process, guarantees a timely Raydium pool launch, and demonstrates your commitment to long-term liquidity. This can significantly contribute to the success of your LBP and the overall health of your token on the Raydium platform.
