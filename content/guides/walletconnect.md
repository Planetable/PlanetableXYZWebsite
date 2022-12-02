+++
title = "Tipping with Ethereum"
description = "Support content creators by tipping with Ethereum."
weight = 31
template = "page.html"
+++

With the release of Planet 0.11 in December 2022, you can now show your support for content creators by tipping with Ethereum. Here's how to use this new feature:

## Connect Wallet

Under the main Planet menu, you'll find a new option called Connect Wallet.

<figure>
  <img src="../../assets/wallet/connect-wallet.png" alt="Connect Wallet" class="screenshot" />
  <figcaption>New menu item: Connect Wallet</figcaption>
</figure>

To use this feature, simply click on the menu item and a QR code will appear. You can then scan the code using a wallet app that supports WalletConnect, such as MetaMask or Rainbow. This will allow you to connect your wallet to the app and access the tipping feature.

<figure>
  <img src="../../assets/wallet/qr-code-example.png" alt="QR Code" class="screenshot" />
  <figcaption>Scan the QR code using a wallet app that supports WalletConnect</figcaption>
</figure>

While browsing ENS dWebsites, you'll see a new tip button in the toolbar. Simply click on the button and choose the amount you'd like to tip. You can select from a range of pre-set amounts to show your support for the content you're enjoying.

<figure>
  <img src="../../assets/wallet/tip-button.png" alt="Tip Button" class="screenshot" />
  <figcaption>Tip Button</figcaption>
</figure>

<figure>
  <img src="../../assets/wallet/tip-tiers.png" alt="Tip Tiers" class="screenshot" />
  <figcaption>Select Amount</figcaption>
</figure>

When you click the Send button, a transaction will appear in your wallet app on your phone. If everything looks correct, simply confirm the transaction on your phone and it will be sent to the Ethereum network. The content creator will then receive the full amount you tipped, without any deductions. This is a simple transfer of funds between two Ethereum addresses. It's that easy!

<figure>
  <img src="../../assets/wallet/sending.png" alt="Sending Transaction" class="screenshot" />
  <figcaption>Sending transaction</figcaption>
</figure>

Once the transaction is confirmed and sent, a browser window will open and display the details of the transaction on the Etherscan website. This will allow you to see the status of the transaction and track its progress on the Ethereum network.

## Wallet Apps

During the development of this feature, we primarily tested with [MetaMask](https://apps.apple.com/us/app/metamask-blockchain-wallet/id1438144202) and [Rainbow](https://apps.apple.com/us/app/rainbow-ethereum-wallet/id1457119021). If your wallet app supports WalletConnect, it should be compatible with this new tipping feature. However, there are some differences in how these two apps support test networks. For example, MetaMask lets you switch between Mainnet, Goerli, and Sepolia, while Rainbow will stay on the initial network you select when you first connect. Keep these differences in mind when using this feature with different wallet apps.