# abloh releases

abloh is a multiplayer terminal IDE built on WezTerm.
People and their coding agents work together in one shell, with glad, the shared record of every decision a team and its agents make, built in from the start.

This repository holds abloh's macOS release downloads.

## Install

**Download the app.**
Get the zip from the [latest release](https://github.com/Vero-Technology/abloh-releases/releases/latest) and unzip it.
abloh is ad-hoc signed, not notarized, so the first launch is blocked by macOS.
Open System Settings, go to Privacy & Security, and click Open Anyway next to the blocked-app message.
That button only shows for about an hour after the blocked attempt; open the app again first if it is gone.
Confirm the prompt and enter your login password.
See [Apple's guide](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unknown-developer-mh40616/mac) for the full steps.
This repeats once per update, since every release is a new app bundle.

**Install from a terminal.**
`curl` and `unzip` never set the quarantine flag a browser download does, so this skips the Open Anyway step entirely.

    curl -LO https://github.com/Vero-Technology/abloh-releases/releases/latest/download/abloh-macos.zip
    unzip abloh-macos.zip
    mv abloh-macos-*/abloh.app /Applications/

**Homebrew.**

    brew install --cask vero-technology/tap/abloh
