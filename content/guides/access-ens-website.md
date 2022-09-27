+++
title = "Access a Website on ENS"
description = "How to access a website on .eth domain."
weight = 31
template = "page.html"
+++

After you have linked IPNS to your ENS domain, you can access your website on .eth domain via these methods.

## ETH.LIMO

ETH.LIMO is a fast and reliable gateway to access websites on .eth domains.

You can append .limo to any .eth domain like this:

<a href="https://planetable.eth.limo" target="_blank">planetable.eth.limo</a>

And it would work in all browsers.

## IPFS Public Gateways

Many IPFS public gateways can load the website on .eth domain by putting the domain in a URL like this:

* <a href="https://ipfs.io/ipns/planetable.eth" target="_blank">ipfs.io/ipns/planetable.eth</a>
* <a href="https://dweb.link/ipns/planetable.eth" target="_blank">dweb.link/ipns/planetable.eth</a>
* <a href="https://cf-ipfs.com/ipns/planetable.eth" target="_blank">cf-ipfs.com/ipns/planetable.eth</a>

Cloudflare also maintains .eth.link and .eth.domains, so you can .link or .domains like this:

* <a href="https://planetable.eth.link/" target="_blank">planetable.eth.link</a>
* <a href="https://planetable.eth.domains/" target="_blank">planetable.eth.domains</a>
 
## Brave Browser

<a href="https://brave.com/" target="_blank">Brave browser</a> has a built-in IPFS node so that it can load IPFS-powered websites natively.

<figure>
  <img src="../../assets/screenshots/brave-ipfs-native.png" alt="Brave has native IPFS support" class="screenshot" />
  <figcaption>Brave browser loads planetable.eth natively</figcaption>
</figure>

To ensure you are using the built-in IPFS node, go to Brave settings, search for IPFS, and change `Method to resolve IPFS resources` to `Brave local IPFS node`.

<figure>
  <img src="../../assets/screenshots/brave-settings-ipfs.png" alt="Brave settings: IPFS" class="screenshot" />
  <figcaption>Brave IPFS settings: Use local node</figcaption>
</figure>

