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

# 🟣 In-depth mechanics

{% hint style="warning" %}
<mark style="color:orange;">A breakdown of the math and mechanics behind</mark> <mark style="color:purple;">**LBP**</mark><mark style="color:orange;">s.</mark>
{% endhint %}

### Understanding weighted math: powering flexible swaps with LaunchPoint

Weighted Math is a groundbreaking innovation that unlocks seamless swaps between any assets in the DeFi space, regardless of their price correlation. This means you can swap between tokens with similar or entirely different values, all within a single LaunchPoint pool.

***

**How does it work?**

Imagine a LaunchPoint pool holding two tokens: Token A and Token B. The price of each token within the pool is determined by three factors:

* **Pool balances:** The amount of each token currently held by the LaunchPoint pool.
* **Pool weights:** Customized weightings assigned to each token, dictating their relative importance within the pool. (Think of these weights as sliders that adjust the price based on how much of each token is present.)
* **Swapped amounts:** The quantity of tokens being exchanged during a swap.

**The math behind the magic:**

LaunchPoint's weighted math equation builds upon the classic constant product formula, but with added flexibility. It can handle pools with more than two tokens and allows for customized weightings beyond a simple 50/50 split.



**Developer tools:**

Developers can leverage the power of Weighted Math through LaunchPoint's open-source implementations:

* **TypeScript:** Utilize the `weightedMath.ts` library for seamless integration into your DeFi projects.
* **Python:** (In Progress) Explore the functionalities offered by the `weightedMath.py` library.

**Spot price calculation:**

Each token pair within a LaunchPoint pool has a unique spot price calculated solely based on the pool's weights and balances. This spot price essentially represents the exchange rate between the two tokens.

The formula considers the balances of both tokens normalized by their corresponding weights.

**Introducing swap fees:**

When swap fees are factored in, the calculation remains similar. We simply use the post-fee input amount (`inAfterFees`) instead of the original input amount (`in`).

**Swap equations:**

These equations determine the amount of one token received when swapping another.

* `outGivenIn`**:** This equation calculates how much of Token B (out) a user receives when swapping a specific amount of Token A (in).

**Important note:**

When calculating this value yourself, remember that the LaunchPoint pool takes a percentage of the input token as a swap fee. The equation uses `inAfterFees` to account for this deduction.

* `inGivenOut`**:** This equation allows users to determine the amount of Token A (in) they need to swap to acquire a desired amount of Token B (out).

**Conclusion:**

Weighted math lays the foundation for powerful and versatile swap functionalities within the DeFi ecosystem. With LaunchPoint's implementation, it opens doors for a wider range of financial interactions by handling diverse asset types and flexible pricing.
