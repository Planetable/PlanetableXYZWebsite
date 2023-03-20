+++
title = "Local Gateway"
description = "IPFS local gateway."
weight = 101
template = "page.html"
+++

Planet includes a recent version of the IPFS node and utilizes it to retrieve and publish information on the IPFS P2P network. This integrated IPFS node provides several useful local ports.

To prevent conflicts with other programs that may utilize these ports, such as a pre-existing IPFS desktop application, we have made minor adjustments to the port numbers.

## Port 18181

This port serves as the local gateway. You can use it to access content on the IPFS P2P network. Below are a few examples.

### Access a specific CID

For example, the <a href="https://github.com/Uniswap/interface/releases/tag/v4.208.0" target="_blank">v4.2.08.0 release of Uniswap</a>:

`CIDv1: bafybeiepywaseoxbaccdblzm6thhqjelkwbamd3guh24wfzba2wwvz6hve`

Access via Local Gateway:

`http://localhost:18181/ipfs/bafybeiepywaseoxbaccdblzm6thhqjelkwbamd3guh24wfzba2wwvz6hve`

<figure>
  <img src="../../assets/screenshots/uniswap-cid.png" alt="Published Folders Dashboard" class="screenshot" />
  <figcaption>Access Uniswap via CID</figcaption>
</figure>

### Access IPNS

IPNS is the naming system utilized by IPFS, which can be accessed through the /ipns/ paths as demonstrated below:

#### ENS

If an ENS has its content hash pointing to a resource on IPFS, it can be accessed through an IPFS gateway in the following manner:

`http://localhost:18181/ipns/vitalik.eth`

<figure>
  <img src="../../assets/screenshots/ipns-vitalik.eth.png" alt="IPNS: vitalik.eth" class="screenshot" />
  <figcaption>IPNS: vitalik.eth</figcaption>
</figure>

#### DNS

If a DNS name has a <a href="https://dnslink.dev/" target="_blank">DNSLink</a> TXT record pointing to a resource on IPFS, it can be accessed through an IPFS gateway:

`http://localhost:18181/ipns/docs.ipfs.tech/`

<figure>
  <img src="../../assets/screenshots/ipns-docs.ipfs.tech.png" alt="IPNS: docs.ipfs.tech" class="screenshot" />
  <figcaption>IPNS: docs.ipfs.tech</figcaption>
</figure>

#### IPNS

[Blogs](@/guides/create-planet.md) and [websites](@/guides/published-folders.md) published from Planet are IPNS. Other Planet users can simply use Follow Planet to receive the latest updates, or these can also be accessed through the local gateway. For example, the IPNS powered <a href="https://app.ens.domains/name/planetable.eth/details" target="_blank">planetable.eth</a> is:

<code>k51qzi5uqu5dgv8kzl1anc0m74n6t9ffdjnypdh846ct5wgpljc7rulynxa74a</code>

It can be accessed via the local gateway:

`http://localhost:18181/ipns/k51qzi5uqu5dgv8kzl1anc0m74n6t9ffdjnypdh846ct5wgpljc7rulynxa74a`

<figure>
  <img src="../../assets/screenshots/ipns-planetable.eth.png" alt="IPNS: planetable.eth" class="screenshot" />
  <figcaption>IPNS: planetable.eth</figcaption>
</figure>

## Port 5981

Kubo, the Go implementation of IPFS, exposes an <a href="https://docs.ipfs.tech/reference/kubo/rpc/" target="_blank">HTTP RPC API</a> that allows you to control the node and run the same commands that you can run from the command line.

You can access this API on port 5981. For example, the following cURL request would return the Identity of the node:

`curl -X POST http://localhost:5981/api/v0/id`

## Origin Isolation

Origin isolation is an important security feature for decentralized app front-ends running on IPFS gateways. So, when you try to access a URL like this:

`http://localhost:18181/ipfs/bafybeiepywaseoxbaccdblzm6thhqjelkwbamd3guh24wfzba2wwvz6hve`

Kubo will return a redirect to transform the URL into this:

`http://bafybeiepywaseoxbaccdblzm6thhqjelkwbamd3guh24wfzba2wwvz6hve.ipfs.localhost:18181/`

However, Safari does not support this kind of URL as of this writing: `*.localhost`. This is a known issue recorded in the WebKit bug tracking system:

[https://bugs.webkit.org/show_bug.cgi?id=160504](https://bugs.webkit.org/show_bug.cgi?id=160504)

To prevent that redirect on Safari, you need to replace `localhost` with `127.0.0.1` so that the redirect will not occur:

`http://127.0.0.1:18181/ipfs/bafybeiepywaseoxbaccdblzm6thhqjelkwbamd3guh24wfzba2wwvz6hve`