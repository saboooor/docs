# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/chargeonuse-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/chargeonuse-addon.md).

## 

What does it do?

Withdraw money from players account in order to use a portal

Requires [Vault](https://www.spigotmc.org/resources/vault.34315/)

## 

How is it configured?

Copy

```
Addon:
  ChargeOnUse:
    Amount: <input1>
    ChargeOnReturn: <input2>
    OneTimePayment: <input3>
    DenyMessage: '<message>'
    ChargeMessage: '<message>'
```

- input1: any integer above 0 to remove from the players balance when they use the portal.
 
- input2: true or false. If its set to false, the plugin will not withdraw money from the player if the world the player came from was the portal world.
 
- input3: true or false. If its set to true, each built portal will charge the player once.
 

[PreviousMessage on use addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/message-on-use-addon) [NextPasted portals addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/pasted-portals-addon)

Last updated 3 years ago