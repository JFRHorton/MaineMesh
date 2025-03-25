# MaineMesh
Welcome to the Maine Mesh project! 

We are buildinig a resilient, off-grid communications network using low-cost LoRa radio devices running the Meshtastic software.

This network provides text messaging, group chats, and weather sensing across the state without the need for internet or cellular access.

## Contact
[MaineMeshNet@gmail.com](mailto:MaineMeshNet@gmail.com)

[Facebook](https://www.facebook.com/groups/570190336078767)

## Getting Started
This guide assumes you already have a Meshtastic-capable device and have completed some basic setup.

For an in-depth guide, check out the [Official Meshtastic Getting Started Guide](https://meshtastic.org/docs/getting-started/)

MaineMesh uses 915MHz LoRa radios. While any compatible radio will work, our current favorites are:
- [The WisMesh pocket for turnkey portable use](https://store.rokland.com/collections/kits/products/wismesh-pocket)
- [The RAKWireless WisBlock starter Kit for DIY-ers](https://store.rokland.com/collections/kits/products/rak-wireless-wisblock-meshtastic-starter-kit)
- [The RAKWireless Mini for Routers and solar nodes](https://store.rokland.com/products/rakwireless-mini-meshtastic-starter-kit-us915-rak19003-4631-sku-115093?variant=42139276247123)

While the default Long Fast channel is present on most nodes, we have a Maine-specific channel. 

This can be added with the following QR code:

![QR Code for MaineMesh MaineNet channel](/channels/mainenet.jpg)


or manually with the following settings:
- **Name**: MaineNet
- **Key Size**: 1 Byte
- **Key**: Vg==


All MaineMesh infrastructure uses **Frequency Slot 20** and the **Long Range - Fast** preset, which is the US standard. 

Devices must have this option configured, otherwise you won't be seen by any other nodes and routers.

## Adding a Router
Want to help cover more of Maine? Great! The backbone of our mesh are router nodes in high places.

Check out the [Router Listing](/router/router_list.md) to see if there is one in your area.

Please send us an email or issue a Git Pull Request against that list to add information:
- **Router Name**: Formatted as **MaineMeshRouter##**
- **Location**: Either specific coordinates or just a town name. This will help plan future routers.
- **Contact**: An email address you're comfortable sharing, in case there is an issue. If you don't want this public, just let us know and we won't include it on the page.
- **Notes**: Any other info, such as hardware type, battery capacity, sensors, etc.

### Routers vs. Repeaters
The preferred setting for backbone devices is ROUTER, instead of REPEATER. 

This is because the ROUTER mode provides additional client telemetry, making planning the mesh easier.

For more info see [Choosing the Right Device Role](https://meshtastic.org/blog/choosing-the-right-device-role/)

### Router Building Guide
TODO

## Disclaimer
We are an independent initiative not officially affiliated with the Meshtastic project.
See the [Meshtastic Licensing Agreement](https://meshtastic.org/docs/legal/licensing-and-trademark/)
