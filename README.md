# ansible-blackarch

Ansible role bootstrap blackarch.

[![Build Status](https://img.shields.io/travis/feffi/ansible-blackarch.svg)](https://travis-ci.org/feffi/ansible-blackarch) [![Github All Releases](https://img.shields.io/github/downloads/feffi/ansible-blackarch/total.svg)](https://github.com/feffi/ansible-blackarch) [![GitHub forks](https://img.shields.io/github/forks/feffi/ansible-blackarch.svg?style=social&label=Fork)](https://github.com/feffi/ansible-blackarch) [![GitHub stars](https://img.shields.io/github/stars/feffi/ansible-blackarch.svg?style=social&label=Star)](https://github.com/feffi/ansible-blackarch) [![GitHub watchers](https://img.shields.io/github/watchers/feffi/ansible-blackarch.svg?style=social&label=Watch)](https://github.com/feffi/ansible-blackarch) [![Twitter Follow](https://img.shields.io/twitter/follow/feffi1.svg?style=social&label=Follow)](https://twitter.com/feffi1) [![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/feffi/ansible-blackarch/blob/master/LICENSE)

## Role Defaults Variables

```yaml
ansible_blackarch: {
  tmp: "BlackArch-1337",
  mirror: "blackarch-mirrorlist",
  keyring: {
    url: "https://www.blackarch.org/keyring/blackarch-keyring.pkg.tar.xz",
    sig: "https://www.blackarch.org/keyring/blackarch-keyring.pkg.tar.xz.sig",
    key: {
      id: "4345771566D76038C7FEB43863EC0ADBEA87E4E3",
      owner: "Evan Teitelman <teitelmanevan@gmail.com>"
    }
  },
  categories: [
    "blackarch",
    #"blackarch-webapp",
    #"blackarch-fuzzer",
    #"blackarch-scanner",
    #"blackarch-proxy",
    #"blackarch-windows",
    #"blackarch-dos",
    #"blackarch-disassembler",
    #"blackarch-cracker",
    #"blackarch-voip",
    #"blackarch-recon",
    #"blackarch-spoof",
    #"blackarch-forensic",
    #"blackarch-crypto",
    #"blackarch-backdoor",
    #"blackarch-binary",
    #"blackarch-networking",
    #"blackarch-misc",
    #"blackarch-exploitation",
    #"blackarch-defensive",
    #"blackarch-wireless",
    #"blackarch-automation",
    #"blackarch-packer",
    #"blackarch-mobile",
    #"blackarch-malware",
    #"blackarch-reversing",
    #"blackarch-sniffer",
    #"blackarch-code-audit",
    #"blackarch-social",
    #"blackarch-honeypot",
    #"blackarch-hardware",
    #"blackarch-fingerprint",
    #"blackarch-debugger",
    #"blackarch-firmware",
    #"blackarch-config",
    #"blackarch-bluetooth",
    #"blackarch-database",
    #"blackarch-cryptography",
    #"blackarch-scan",
    #"blackarch-automobile",
    #"blackarch-decompiler",
    #"blackarch-nfc",
    #"blackarch-tunnel",
    #"blackarch-drone",
    #"blackarch-radio",
    #"blackarch-keylogger",
    #"blackarch-stego",
    #"blackarch-unpacker",
    #"blackarch-anti-forensic",
    #"blackarch-ids",
    #"blackarch-spoff",
    #"blackarch-gpu"
  ]
}
```

Example:

```yaml
- hosts: all
  vars:
    ansible_blackarch:
      tmp: "BlackArch-1337"
      mirror: "blackarch-mirrorlist"
      keyring:
        url: "https://www.blackarch.org/keyring/blackarch-keyring.pkg.tar.xz"
        sig: "https://www.blackarch.org/keyring/blackarch-keyring.pkg.tar.xz.sig"
        key:
          id: "4345771566D76038C7FEB43863EC0ADBEA87E4E3"
          owner: "Evan Teitelman <teitelmanevan@gmail.com>"
      categories:
        - "blackarch"
        #- "blackarch-webapp"
        #- "blackarch-fuzzer"
        #- "blackarch-scanner"
        #- "blackarch-proxy"
        #- "blackarch-windows"
        #- "blackarch-dos"
        #- "blackarch-disassembler"
        #- "blackarch-cracker"
        #- "blackarch-voip"
        #- "blackarch-recon"
        #- "blackarch-spoof"
        #- "blackarch-forensic"
        #- "blackarch-crypto"
        #- "blackarch-backdoor"
        #- "blackarch-binary"
        #- "blackarch-networking"
        #- "blackarch-misc"
        #- "blackarch-exploitation"
        #- "blackarch-defensive"
        #- "blackarch-wireless"
        #- "blackarch-automation"
        #- "blackarch-packer"
        #- "blackarch-mobile"
        #- "blackarch-malware"
        #- "blackarch-reversing"
        #- "blackarch-sniffer"
        #- "blackarch-code-audit"
        #- "blackarch-social"
        #- "blackarch-honeypot"
        #- "blackarch-hardware"
        #- "blackarch-fingerprint"
        #- "blackarch-debugger"
        #- "blackarch-firmware"
        #- "blackarch-config"
        #- "blackarch-bluetooth"
        #- "blackarch-database"
        #- "blackarch-cryptography"
        #- "blackarch-scan"
        #- "blackarch-automobile"
        #- "blackarch-decompiler"
        #- "blackarch-nfc"
        #- "blackarch-tunnel"
        #- "blackarch-drone"
        #- "blackarch-radio"
        #- "blackarch-keylogger"
        #- "blackarch-stego"
        #- "blackarch-unpacker"
        #- "blackarch-anti-forensic"
        #- "blackarch-ids"
        #- "blackarch-spoff"
        #- "blackarch-gpu"

  roles:
    - { role: ansible-blackarch }
```
