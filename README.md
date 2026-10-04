# The Scoop bucket of Burnout and HotDogStand

[Burnout](https://github.com/Stiven-Gjekaj/burnout) writes a bootable USB
drive from the command line. The commands are the same on Windows, on macOS
and on Linux.

## Install

    scoop bucket add stiven-gjekaj https://github.com/Stiven-Gjekaj/scoop-bucket
    scoop install stiven-gjekaj/burnout

The manifest installs the Windows binary of the release, for x86_64 and for
arm64. Scoop checks each download against its SHA-256. Burnout writes a drive
only from a shell that runs as Administrator.

Burnout erases the drive that you give it, and nothing undoes that. Read
[TERMS.md](https://github.com/Stiven-Gjekaj/burnout/blob/main/TERMS.md)
before you run it.

## HotDogStand

[HotDogStand](https://github.com/Stiven-Gjekaj/HotDogStand) is a ticket
manager on your own computer, with the look of Windows 7.

    scoop bucket add stiven-gjekaj https://github.com/Stiven-Gjekaj/scoop-bucket
    scoop install stiven-gjekaj/hotdogstand

The manifest installs the Windows package of the release, for x86_64, and
puts HotDogStand in the Start menu. Scoop checks the download against its
SHA-256. `scripts/scoop-manifest.sh` in the HotDogStand repository writes
`bucket/hotdogstand.json` from the `SHA256SUMS` of each release.

## Where the manifest comes from

`scripts/scoop-manifest.sh` in the Burnout repository writes
`bucket/burnout.json` from the `SHA256SUMS` of each release. Change the
script, and not the manifest. A person writes each commit here. No bot pushes
to this bucket.

Report a problem in the
[issues of Burnout](https://github.com/Stiven-Gjekaj/burnout/issues).
