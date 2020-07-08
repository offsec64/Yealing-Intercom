# Yealink Intercom
[![Tested On Yealink T42s](https://img.shields.io/badge/Tested%20On-Yealink%20T42s-green)](https://github.com/offsec64/yealink-intercom/)

## On the phone(s) you want to be able to speak into:

* First, Press `Menu` on the homescreen and navigate to `Features>DSSKey`.
* Go to whichever line item you want the intercom to be on.
* Set the following (use the arrow keys):
  * _Type:_ Key Event
  * _Key Type:_ Multicast Paging
  * _Label:_ Whatever you want, I did Intercom
  * _Address:_ 224.5.6.20:10008
  * _Channel:_ 0

## On the phone(s) you want to use as the intercom:

* Log in to the web interface and navigate to `Directory`, then on the sub menu, go to `Paging`.
* Set `Igonre DND` if you want the intercom to work even if DND is on (the numbers are for priority).
* Under the IP Addresses list, go to `1 IP Address` and under Listening Address, type `224.5.6.20:10008`
* Under Label, set what you want it do display when the intercom is on, I did Intercom!
* Leave the channel at 0.
* In the `Paging List`, copy and paste the Paging Address and Label from above.

## To use the intercom:
Press the DSS Key with the label you set, and your voice will be on the other phone(s)!

> The address and channel are what Yealink says to use for the intercom.

