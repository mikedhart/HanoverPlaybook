---
title: Security
section: guides
layout: page
---

A guide for practicing safe web and keeping our partners's data safe.

## Think

Security is important, and you can't practice these guidelines without
understanding them. Make sure you understand each guideline, why it exists, and
how to follow it.

Failing to follow these guidelines will likely put you, your team, and your
deployed services at risk of compromise or loss of privacy.

## Secure Employee Access and Communication

The following guidelines apply to how you as an individual
secure access to your systems (laptop, accounts, etc.)
and communication (email, etc.).

### Using Passwords

* Use a unique password for every account you create.
* Use a tool like [LastPass](https://www.lastpass.com) or
  [1password](https://1password.com) to generate random passwords.
* Never paste your password as plain text. If you have to share a password with someone then use the [share functionality](https://blog.lastpass.com/2016/01/tips-for-securely-sharing-passwords.html/) from within your password manager.

### Encryption

* Ensure [disk encryption][disk] is enabled on your Mac.
* Don't share your private key with anyone, including services like Keybase.
* Keep at least one backup of your private key and revocation certificate in a
  secure location, such as a thumb drive.

[disk]: https://support.apple.com/en-gb/HT204837

## Physical Security

The following guidelines apply to how we physically secure
our laptops and mobile devices that may contain customer or user data.

The word "device" relates to any device you use to access any of our or our partner's data.

* Lock your device when you are away from it.
* Ensure that your device requests a password on wake.
* Don't leave your devices unattended in an unsecured area.
* Ensure that your device can be remotely wiped:
  - [Apple][applewipe]
  - [Android][androidwipe]
* If you regularly work in public locations such as coffee shops, trains or planes, use a privacy filter.

[applewipe]: https://support.apple.com/en-us/HT204756
[androidwipe]: https://support.google.com/accounts/answer/6160491?hl=en

## Application Security

The following guidelines apply to how we develop
software on behalf of ourselves and partners.

### Transmitting Information

* Don't accept passwords or session tokens over HTTP.
* Use HTTPS for **all** web traffic.
* Use HTTPS in the beginning; it's harder to introduce later.
* Use HTTPS redirects for HTTP traffic.
* Avoid protocol-relative URLs.

### Storing Information

* Don't log passwords.
* Don't store passwords in plain text.
* Don't hash passwords using a reversible cipher.

### Preventing Vulnerabilities and Regressions

During active development of a codebase,
track security alerts in Continuous Integration builds
with tools such as [Bundler Audit].

## Handling Vulnerabilities

The following guidelines apply to how we handle security incidents.

### Reporting

When someone finds a possible security issue in our software,
we encourage them to report it to our <support@cleversteam.com> email address.

When an email comes in through this channel,
reply quickly with confirmation.

### Reviewing, Logging and Following Up

When a message comes in,
post the exchange to a new [Slack] thread in the `#security` channel,
and keep the thread updated with new messages as they appear.

[Slack]: https://slack.com/

Further discussion of security takes place in the `#security` channel in Slack.
