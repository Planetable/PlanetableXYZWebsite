+++
title = "Link a Website to .bit"
description = "Add IPNS built with Planet to .bit DWeb record."
weight = 40
template = "page.html"
+++

<a href="https://app.did.id/explorer?inviter=planetable.bit" target="_blank">.bit</a> is a blockchain based identity system powered by <a href="https://www.nervos.org/" target="_blank">Nervos Network</a> blockchain.

It supports several types of DWeb records, including IPNS. You can add an IPNS built with Planet to your .bit domain.

## Step 1 · Copy IPNS

Right-click your website under My Planets and select Copy IPNS. You will get its IPNS in the pasteboard, and it will be a long string that starts with `k51`.

<figure>
  <img src="../../assets/screenshots/copy-ipns.png" alt="Copy IPNS" class="screenshot" />
  <figcaption>Copy IPNS</figcaption>
</figure>

## Step 2 · Add DWeb Record

Go to the [.bit Manage dashboard](https://data.did.id), click Manage Data, and add a new record under DWeb. Select `IPNS` as key, and provide the value you get from Copy IPNS.

<figure>
  <img src="../../assets/screenshots/dotbit-add-ipns.png" alt=".bit Add IPNS" class="screenshot" />
  <figcaption>Copy IPNS</figcaption>
</figure>

And save the change. .bit does not need you to pay gas when you update the records.

## Step 3 · Access

After the DWeb record becomes effective, you can access your website with .bit.cc public gateway like this:

<a href="https://planetable.bit.cc" target="_blank">planetable.bit.cc</a>

You can also use it in Follow Planet.

<figure>
  <img src="../../assets/screenshots/dotbit-follow.png" alt="Follow .bit" class="screenshot" />
  <figcaption>Follow .bit</figcaption>
</figure>
