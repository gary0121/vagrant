---
page_title: "vagrant connect - Command-Line Interface"
sidebar_current: "cli-connect"
---

# Connect

**Command: `vagrant connect NAME`**

The connect command compliments the
[share command](/docs/cli/share.html) by enabling access to shared
environments. You can learn about all the details of Vagrant Share in the
[Vagrant Share section](/docs/share).

The reference of available command-line flags to this command
is available below.

## Options

* `--disable-static-ip` - The connect command will not spin up a small
  virtual machine to create a static IP you can access. When this flag is
  set, the only way to access the connection is to use the SOCKS proxy
  address outputted.

* `--static-ip IP` - Tells connect what static IP address to use for the virtual
  machine. By default, Vagrant connect will use an IP address that looks
  available in the 172.16.0.0/16 space.

* `--ssh` - Connects via SSH to an environment shared with
  `vagrant share --ssh`.