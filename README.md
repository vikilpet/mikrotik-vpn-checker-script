**This script is obsolete. The new script is better than this one in every way**:

https://github.com/vikilpet/mikrotik-interface-check


# Mikrotik VPN Checker

### Features
- any amount of ping targets
- any amount of interfaces
- reconnect interface and check if it became working
- show failed hosts in log

### How It Works
You have some VPN interfaces called almost the same \(VPN1, VPN2 etc.\)

You have routes through this interfaces with different distance so if one of them become unactive another will become active.

This script will find all interfaces that will match mask in *IntMask* variable and ping all hosts in *Hosts* variable through every interface. If successful ping percentage will less than *PingResult* variable then corresponding route will be disabled (or enabled in case of good ping).

### Prerequisites
RouterOS v6

### Installing
Save script in */system scripts* and run it with scheduler as offten as you want.

Variable *ScriptName* should have actual script name to protect from concurrent running.


#### \*\*\*
Feel free to ask questions or correct my spelling mistakes.