+++
title = "Link a Website to ENS"
description = "Link the website built with Planet to your ENS."
weight = 30
template = "page.html"
+++

After you have created a website and added a post, it will get published to IPFS, and you will get its unique ID, also known as IPNS. IPNS can then be used to link to your ENS.

Right-click your website under My Planets and select Copy IPNS. You will get its IPNS in the pasteboard, and it will be a long string that starts with `k51`.

Navigate to your domain on the ENS app, and click "Add/Edit Record" to start changing. And you can paste your IPNS to the Content section. Be sure to add ipns:// before the `k51...` string like this:

<figure>
  <img src="../../assets/screenshots/set-contenthash.png" alt="Set contenthash" class="screenshot" />
  <figcaption>Set contenthash for your ENS domain</figcaption>
</figure>

Then scroll to the bottom of the page and click Confirm. There will be a gas fee prompt from MetaMask because this is an interaction with the ENS smart contract to change a field of your domain on the Ethereum blockchain.