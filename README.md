# WWDC 2018 Lab Questions

Here are some topics for discussion in the WWDC Labs.


## codesign "unknown error -1=ffffffffffffffff"

Command should give some clue as to the cause of the error.

https://github.com/openbakery/gradle-xcodePlugin/pull/375

- [ ] Radar submitted?


## security set-key-partition-list docs suck

This is a cop-out:

> See output of "security dump-keychain" for examples.

```
set-key-partition-list [-S <partition list (comma separated)>] [-k <keychain password>] [options...] [keychain]
    Sets the "partition list" for a key. The "partition list" is an extra parameter in the ACL which limits access to the key based on an application's code signature. You
    must present the keychain's password to change a partition list. If you'd like to run /usr/bin/codesign with the key, "apple:" must be an element of the partition list.

    -S partition-list
                    Comma-separated partition list. See output of "security dump-keychain" for examples.
    -k password     Password for keychain
    -a application-label
                    Match "application label" string
    -c creator      Match creator (four-character code)
    -d              Match keys that can decrypt
    -D description  Match "description" string
    -e              Match keys that can encrypt
    -j comment      Match comment string
    -l label        Match label string
    -r              Match keys that can derive
    -s              Match keys that can sign
    -t type         Type of key to find: one of "symmetric", "public", or "private"
    -u              Match keys that can unwrap
    -v              Match keys that can verify
    -w              Match keys that can wrap
```

- [ ] Radar submitted?


## ClassKit for enterprise

- Want TouchID for unlocking and identifying/switching users
- Might be some features in iOS 11.4

Multi user devices
* Touch id
* Classkit
* shared devices

- [ ] Radar submitted?

## macOS password dialogs

GUI dialogs triggered from CLI commands are just silly. They fail with a generic error when there is not window session (SSH and user not logged into console), but if there is there isn't a way to supply the password to the GUI from a script.

- Any way to prevent?
- Provide auth via CLI

- [ ] Radar submitted?


## AD bind pre-login

- search for existing radars to dup
* enterprise connect is post-login

- [ ] Radar submitted?


## Subsidiary dev program

We would like to be able to have several separate developer programs to create different KP "brands" (or labels) in the public app store.
However, we would want one central team to manage them.

- example: Ford vs Lincoln
- Center for Health Research
  - dev program request denied
  - told to use main KP dev program
  - can we still register a program for them?
- KP School of Medicine
  - also will want to release apps
- Perhaps umbrella brand for Kaiser Research

- [ ] Radar submitted?


## Hypervisor Framework

- How to use
- Any vendors building container products using it?
  - [Veertu](https://veertu.com/) Anka

- [ ] Radar submitted?
