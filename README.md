# PortaKube

**Building a portable K3s cluster for fun and ~~profit~~ fun.

This repo contains docs, scripts and info for PortaKube, my portable K3s battery-powered LTE-infused portable computing project.

There are many examples of portable kubernetes ARM clusters out there. This is another one of those clusters, but I wanted to change a couple of things up. Most of the examples I could find were powered by AC mains and limited to connectivity via WiFi or LAN. 

That's great and all, but we can do better.

**Let's free our cluster and give it the ability to go anywhere!** To do so, we'll need to give it some important ingredients:
- Batteries!
- LTE connectivity!
- A case for protection (time allowing...)

Before we get started, you may be wondering 'why would you do this?' A few reasons:
- To learn
- Just because
- Remote sensor-based data collection w/ first-class data CLI tools
- Portable distributed clustered computing at the edge
- For fun

This isn't a 100% practical project, but the things learned from it can be applied to actual products or services. For example, as computing is increasingly more mobile and moving more ARM-based:
- How do we handle graceful degradation at the edge? 
- How do we optimize for battery-only scenarios?
- how can we break up complex workloads across edge compute devices or clusters and the cloud?
- How do we deploy autonomously to make sure remote devices are always up to date?

Ok, on to the fun!

## Shopping List
We'll need a few components to get this off the ground. Size your cluster as you like, I went with 4x:
- [4x Raspberry Pi 3b+](https://www.amazon.com/ELEMENT-Element14-Raspberry-Pi-Motherboard/dp/B07BDR5PDW)
- [4x 32gb MicroSD cards](https://www.amazon.com/gp/product/B06XWN9Q99/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&psc=1)
- [Spacers/standoffs](https://www.amazon.com/gp/product/B01L06CUJG/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&psc=1)
- [4x Battery pack expansion boards](https://www.amazon.com/gp/product/B079M9YQP8/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1)
- [4x micro-usb cables](https://www.amazon.com/gp/product/B07PFZDQP6/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&psc=1)
- [Power brick](https://www.amazon.com/Anker-Charger-PowerPort-iPhone-Galaxy/dp/B00P936188)
- [Sixfab Pi LTE Base Shield](https://sixfab.com/product/raspberry-pi-3g-4glte-base-shield-v2/)
- [Sixfab LTE Modem (pick the right one for your carrier/locale)](https://sixfab.com/product/quectel-ec25-mini-pcle-4glte-module/)
- A data SIM for your carrier
- Velcro/wire-ties etc.
