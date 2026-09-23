# KeeFortress

A Windows-first, open-source password manager project based on [KeePassXC](https://github.com/keepassxreboot/keepassxc), with a modern interface and flexible organization for passwords and secure notes.

## Project status

**Early development.** The KeeFortress interface currently exists as a design prototype. It has not yet been added to the desktop app, and no KeeFortress release has been tested for everyday use.

The repository starts from KeePassXC's source code. Existing feature lists, build instructions, and release notes came from KeePassXC. They do not mean that KeeFortress has been tested or released. The prototype uses temporary sample data and is not a place to store real passwords or other login details.

## Our direction

KeeFortress aims to use KeePassXC's existing code for protecting and saving vaults, with an interface that makes everyday tasks easier.

Planned interface features include:

- A compact Home with favorites, frequently used entries, and recent changes.
- Expandable password categories and a separate Secure Notes area.
- More than one password in an entry, with one clearly marked as the password used to log in.
- Organized recovery codes, attachments, and entry history.
- Archive for old login details worth keeping, and Trash that would keep deleted entries for 30 days.
- Clear vault creation, locking, and backup settings.

These are development plans, not a list of completed features. See the [roadmap](ROADMAP.md).

## Vaults and compatibility

The goal is to use local, encrypted `.kdbx` vault files and preserve compatibility with KeePassXC. One vault would be open at a time in the proposed interface. No KeeFortress online account or hosted storage service is planned for the initial version.

Formatted notes and extra information saved with entries need testing before release. We will document how they appear in other apps that open KDBX vault files and verify that opening and saving a vault does not unexpectedly lose data. See [how the app will work](docs/keefortress/ARCHITECTURE.md).

## Platforms and builds

Windows is the first target. macOS is a later goal; iOS is a possibility that needs more planning. Support for other operating systems has not been decided.

The first step is to build the original KeePassXC app for Windows. Then we will add opening, editing, saving, and locking vaults through the KeeFortress interface. See [development](docs/keefortress/DEVELOPMENT.md). The inherited [INSTALL.md](INSTALL.md) explains how to build KeePassXC.

## Participate

- Report ordinary bugs or suggest improvements in [KeeFortress Issues](https://github.com/nrtak/keefortress/issues).
- Read the [contribution guidelines](.github/CONTRIBUTING.md) before submitting changes.
- Follow the [code of conduct](CODE-OF-CONDUCT.md).
- Report security weaknesses by following [SECURITY.md](SECURITY.md), never in a public issue.

## Relationship to KeePassXC

KeeFortress is an independent fork. It is not an official KeePassXC release and is not presented as approved by the KeePassXC team. KeePassXC maintainers are not responsible for KeeFortress changes, support, or releases.

We plan to review KeePassXC updates regularly, bring in relevant fixes, and test them. KeeFortress will not update automatically when KeePassXC releases a new version. See [bringing in KeePassXC updates](docs/keefortress/UPSTREAM.md).

## License and acknowledgments

KeeFortress keeps the GNU GPL version 2 or, at your option, version 3 license used by KeePassXC. Some files from other projects have their own license terms. See [COPYING](COPYING), [GPL-2](LICENSE.GPL-2), [GPL-3](LICENSE.GPL-3), and the other license files in this repository.

Original copyright notices, source headers, and third-party notices are retained. See [acknowledgments](ACKNOWLEDGMENTS.md). The inherited [CHANGELOG.md](CHANGELOG.md) records KeePassXC release history; KeeFortress changes are tracked [separately](docs/keefortress/CHANGELOG.md).
