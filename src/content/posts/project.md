---
title: A Project Proposal - Part 1
description: meow I want to make a password manager :3
pubDate: Dec 24 2025
---

# Context
A password manager is software that enables convenient usage of passwords and other authenitcation related measures by allowing users to easily generate, fill and store passwords securely. 

<br>

Instead of a user having to remember many different passwords for different applications, or compromise on security by reusing passwords, a password manager allows one to remember a "master password" to access all other passwords.

# Existing Systems

There are many existing solutions for password managers.

<br>

Some examples include:
- KeePassXC
- 1Password
- Browser-provided Password Managers

## KeePassXC
> "KeePassXC is a modern, secure, and open-source password manager that stores and manages your most sensitive information." 
>
> <br>
>
> -- KeePassXC [website](https://keepassxc.org/)

<br>

KeePassXC excels as an offline password manager. By saving all passwords in a local encrypted .kdbx file, KeePassXC securely stores passwords.

<br>

KeePassXC also contains useful tools, such as Time-based one-time password (TOTP) generation, password generation, and browser autofill.

<br>

However, whilst KeePassXC excels in an offline, local solution, it lacks a dedicated network sync between devices, meaning that workarounds are needed.

## 1Password
1Password is a proprietary solutiom that contains many features, including syncing between devices. 1Password provides enterprise and personal password managers, in addition to other authenitcation-related services.

<br>

1Password, like KeePassXC excels at being an offline password manager.

<br>

In addition to this, 1Password offers the ability to sync passwords cross-platform, including Android and iOS applications. 

<br>

1Password also includes useful tools including password generation and browser autofill.

<br>

However, 1Password is a proprietary, closed source solution, and requires payment after their free trial. Although they release security audit reports, many of these are locked behind a paywall / account and may not be available publicly.

## Browser-provided Password Managers
Most modern browsers, including Chrome and Firefox, ship with a built-in password manager.

<br>

Because it is part of the browser, these password managers are well integrated and function exceptionally for websites. 

<br>

However, the implementation of these password managers lacks security because as a part of the browser, it is subject to critical design restrictions that opens up many attack vectors. In fact, they is so insecure that most common, untargeted malware will automatically attempt to steal passwords from a browser-provided manager, and often succeed. 

<br>

See:
- [a Sophos report about Qilin ransomware](https://www.sophos.com/en-us/blog/qilin-ransomware-caught-stealing-credentials-stored-in-google-chrome)  
- [the Raven stealer GitHub repository](https://web.archive.org/web/20250804090707/https://github.com/luis22d/Raven-Stealer)
- [a Cyfirma writeup on the Raven stealer malware](https://www.cyfirma.com/research/raven-stealer-unmasked-telegram-based-data-exfiltration/)

<br>

In addition to these security limitations, these password managers are usually unable to sync across devices.

# Foreword
Thus, it is evident that a new, FOSS alternative that aims to make up for these shortcomings and preserves their strengths is needed.
