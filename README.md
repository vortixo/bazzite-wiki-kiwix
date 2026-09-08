# Bazzite Wiki Kiwix

Automatically builds an offline Kiwix ZIM archive from the Bazzite documentation.

## What it does

GitHub Actions periodically checks the upstream Bazzite documentation repository, builds the MkDocs site, converts the generated static site to an OpenZIM archive, validates the archive, and publishes it as the `bazzite-wiki.zim` asset of a rolling GitHub Release.

The workflow can also be started manually.

## Download

Open the repository's **Releases** page and download the latest `bazzite-wiki.zim` asset. Open that file with Kiwix.

## Update policy

The scheduled workflow checks upstream every day. It only publishes a new release when the upstream documentation commit has changed. Pushes to this builder repository and manual runs also build the archive.

## Source

Upstream documentation: https://github.com/ublue-os/docs.bazzite.gg
