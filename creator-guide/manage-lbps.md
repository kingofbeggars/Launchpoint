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

# ⌨️ Manage LBPs

{% hint style="info" %}
A step-by-step guide to explain how to manage LBPs in LaunchPoint.
{% endhint %}

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption><p>"If you want your mind to find what it's looking for quickly, just multiply your options!"</p></figcaption></figure>

***

**->** After the LBP raise has been completed or duration finished, the creator can then go to the pool management menu via the `Manage Pool` button from the main LBP page. It will look like this:

<figure><img src="../.gitbook/assets/image (10).png" alt="" width="466"><figcaption><p>Finished LBP management menu.</p></figcaption></figure>

**->** After the LBP has been concluded a Raydium pool will be created with the locked amounts, with you as the creator, and the LP tokens will be burned automatically. After that, you will receive all the rest of the SOL and tokens in the pool, minus the fee on the raised amount of SOL.

**->** In order for the Raydium pool to be created, an Openbook (Serum) Market Id is required. If one isn't provided, we'll create one automatically. **This requires multiple transactions, and you need to sign all in order!**

{% hint style="warning" %}
**Note**: Make sure you have a balance of at least **3 SOL** in your creator wallet in order to successfully execute all the transactions that will appear in order as specified in the paragraph above!
{% endhint %}

<figure><img src="../.gitbook/assets/image (11).png" alt="" width="464"><figcaption><p>LBP results summary and claimable amounts.</p></figcaption></figure>

**->** After signing **all the remaining transactions** for the Openbook Market ID creation (Not applicable if the creator already provides one) the pool will be created on Raydium and the funds claimed!
