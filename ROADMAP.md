# KeeFortress roadmap

These are the planned steps. There are no promised release dates. Each step needs working code and testing, not just a finished design.

## 1. Build the starting app

- Record the exact KeePassXC version and commit we start from. A commit identifies a saved set of code changes.
- Build the original app for Windows and run the relevant KeePassXC tests.
- Set up GitHub Actions to build the app and provide test versions to download.
- List the tools needed, license terms, and known limitations.

## 2. Make the basic KeeFortress interface work

- Open and unlock a vault using KeePassXC's existing code.
- Browse, search, create, and edit password entries.
- Save and lock the vault using KeePassXC's existing code.
- Clearly explain errors and warn about unsaved edits.
- Check that a sample vault can be opened, edited, and saved in both apps without losing information.

## 3. Add organization and entry details

- Add Home, favorites, categories, and extra password fields.
- Decide how recovery codes are saved and marked as used.
- Add Archive and Trash while keeping entry history.
- Remove entries after 30 days in Trash. If the vault is closed, wait until it is next unlocked and can be saved safely.
- Explain that older backups may still contain deleted entries.

## 4. Add Secure Notes and settings

- Add text formatting, simple tables, and charts, and explain how they are saved.
- Check what happens to notes when someone edits the vault in another app.
- Connect backup, locking, clipboard, and history settings to working features.
- Check keyboard use, accessibility, and different Windows text and display sizes.

## 5. Prepare for release

- Test saving failures, restoring backups, opening vaults in other apps, and handling private information.
- Review changes that affect security and fix problems that would make a release unsafe.
- Set up private security reporting and explain which versions will receive updates.
- Update the app name, installer details, and links used to check for updates.
- Publish build instructions, release notes, and details of how each download was made.
- Decide how to sign installers so Windows can identify the publisher, and how users will receive updates.

## Later possibilities

macOS support, browser extension support, and a closer look at what an iOS app would require. No release dates are promised.
