+++
title = "DWebServices.xyz for Hosted IPNS Records"
description = "Use API from DWebServices.xyz for hosted IPNS records."
weight = 2010
template = "page.html"
+++

<a href="https://dwebservices.xyz/" target="_blank">DWebServices</a> is an IPNS record hosting service. When the integration is enabled in Planet, each time you update your website, the latest CID will be sent to DWebServices to be updated in the IPNS record hosted there.

To start, first, you can sign up with your Ethereum wallet. The service can detect ENS domains already in the wallet, or you can add any domain to the dashboard. Then when you edit planet, you will find a section to enter the domain and API key here:

<figure>
  <img src="../../assets/screenshots/dwebservices-api-key.png" alt="DWebServices.xyz API Key" class="screenshot" />
  <figcaption>Set DWebServices.xyz API Key</figcaption>
</figure>

Then, in addition to the built-in IPNS record in Planet, you will now have another IPNS record hosted with DWebServices. The hosted IPNS record usually has better discoverability because it's on a well-connected server. That is especially useful for users running Planet from their laptops since laptops are not meant to be running 24x7 as servers.

You can set that hosted IPNS record as your ENS contenthash or .bit dWeb record too.