# Security policy

## Development status

KeeFortress is in early development. There is no supported KeeFortress release or promised security-update schedule yet. The interface prototype uses sample data; it does not provide encrypted storage.

Using KeePassXC code does not mean our changes have been checked for security. Reviews and security badges for KeePassXC do not cover KeeFortress.

## Report a security weakness privately

Do not publicly share details of a security weakness, real passwords, vault files, recovery codes, key files, or private logs in a public issue or pull request.

If available, use **Security → Advisories → Report a vulnerability** in [this repository](https://github.com/nrtak/keefortress/security). Availability depends on the repository owner enabling private vulnerability reporting.

If that control is unavailable, we have not listed another private way to report a problem yet. You may open an issue asking only for a private contact method, without describing the security weakness or sharing private information. Wait until the project owner provides a private way to contact them before sharing details.

When you can report privately, tell us which version and operating system you used, what happened, what you expected, and why the problem matters. Explain how to make it happen again using made-up examples instead of real passwords or personal information. We cannot promise a reply within a set time and do not currently offer rewards for finding security problems.

If you have also confirmed the problem in the original KeePassXC app, follow [KeePassXC's security policy](https://github.com/keepassxreboot/keepassxc/security/policy). Problems caused by KeeFortress changes should be reported to KeeFortress.

## Before a supported release

Before a supported release, the project team must check that private reporting works, list the versions receiving support, explain how security updates will arrive, and review changes that affect security. Details that could help someone misuse a security weakness should stay private while a fix is prepared.
