# Troubleshooting

Bridge transactions can take some time \(hours in extreme cases\) to complete depending on Ethereum mainnet congestion.  Try these actions first if your transaction has been **pending for 10 minutes or more** \(and you don't want to wait any more time\). Usually, a transaction will resolve itself after some time, but there are things you can do to speed up the process. Actions differ depending on if you are transferring from Dai to xDai or xDai to Dai.

{% hint style="info" %}
An update to the current bridge UI is in process. The following are interim solutions while we work on these upgrades.
{% endhint %}

## Dai to xDai

8 block confirmations are required to ensure a transaction is final and xDai can be minted to your account. If Ethereum is congested, it may take many more blocks for your transaction to be queued. If your transaction is stuck in pending for a long time, you can opt try to speed it up by selecting the pending transaction in MetaMask, clicking Speed Up, then paying the additional gas to try and get it through more quickly. Otherwise, it will likely be in a pending state until the congestion breaks up.

![](../../.gitbook/assets/speedup.jpg)

## xDai to Dai

If your transfer is processing for more than 10 minutes ****and you have not received your Dai back, you may want to process it manually, bypassing some of the oracles components and submitting the signatures yourself. This will incur gas fees but will speed up the transaction - so you can pay now or wait for the tx to go through with a 0 fee.

To start, copy the tx hash of the pending transaction on xDai. You can copy this from an xDai connected instance of MetaMask.

![Click on the pending transaction to get the tx hash](../../.gitbook/assets/mm2.jpg)

Go to [https://k1rill-fedoseev.github.io/manual-submit-signatures/](https://k1rill-fedoseev.github.io/manual-submit-signatures/) and set your MetaMask Wallet to the **Main Ethereum Network**

1. Paste pending tx hash.
2. Click Submit.
3. MetaMask will activate to process the new tx. Gas price should populate...If not, or if you want to ensure the tx goes through quickly, check current gas prices to decide your limit. [https://ethgas.watch](https://ethgas.watch/) provides an aggregated price feed.
4. Click Confirm to process.

![](../../.gitbook/assets/kirill1.jpg)





