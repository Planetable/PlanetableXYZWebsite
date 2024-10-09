+++
title = "Link a Website to Solana Name (.sol)"
description = "Add IPNS built with Planet to .sol IPNS record."
weight = 31
template = "page.html"
+++

Solana Name Service (<a href="https://sns.id/" target="_blank">sns.id</a>) is an identity system running on the Solana blockchain. It supports adding an IPNS record to the name, and furthermore, there is a gateway to access `.sol` names with IPFS/IPNS records.

You can register your Solana name at <a href="https://sns.id/" target="_blank">sns.id</a>. <a href="https://phantom.app/" target="_blank">Phantom</a> wallet app is recommended, and have some USDC in the wallet.

## Step 1 · Copy IPNS

Right-click your website under My Planets and select Copy IPNS. You will get its IPNS in the pasteboard, and it will be a long string that starts with `k51`.

<figure>
  <img src="../../assets/screenshots/copy-ipns.png" alt="Copy IPNS" class="screenshot" />
  <figcaption>Copy IPNS</figcaption>
</figure>

## Step 2 · Set IPNS Record

Open your name's records page, click `Edit Records`.

<figure>
  <img src="../../assets/screenshots/sol-edit-records.png" alt="Edit Records" class="screenshot" />
  <figcaption>.sol: Edit Records</figcaption>
</figure>

Find the row named `IPNS`, and paste the IPNS string (it starts with `k51`).

<figure>
  <img src="../../assets/screenshots/sol-ipns-record.png" alt=".sol IPNS Record" class="screenshot" />
  <figcaption>.sol: IPNS Record</figcaption>
</figure>

And click `Save Changes`.

## Step 3 · Access

Solana is a fast blockchain, capable of updating your record in less than a second. Once your IPNS record is saved, you can access your website using the <a href="https://sol.build/" target="_blank">sol.build</a> public gateway.

<a href="https://planetable.sol.build/" target="_blank">planetable.sol.build</a>