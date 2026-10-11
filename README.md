# The Scoop bucket of Burnout, HotDogStand, AllTheTools and OnyxDiskInfo

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

## AllTheTools

[AllTheTools](https://github.com/Stiven-Gjekaj/AllTheTools) is one command,
`att`, with twenty tools that one system has and the other two do not, such
as lsusb, f3probe and caffeinate.

    scoop bucket add stiven-gjekaj https://github.com/Stiven-Gjekaj/scoop-bucket
    scoop install stiven-gjekaj/allthetools

The manifest installs the Windows binary of the release, for x86_64 and for
arm64. Scoop checks the download against its SHA-256. `att probe` and
`att surface` need a shell that runs as Administrator.
`scripts/scoop-manifest.sh` in the AllTheTools repository writes
`bucket/allthetools.json` from the `SHA256SUMS` of each release.

## OnyxDiskInfo

[OnyxDiskInfo](https://github.com/Stiven-Gjekaj/OnyxDiskInfo) reads the
health of every disk, and tests, formats and erases it. The command line is
`onyx`, and the app is in the style of CrystalDiskInfo.

    scoop bucket add stiven-gjekaj https://github.com/Stiven-Gjekaj/scoop-bucket
    scoop install stiven-gjekaj/onyxdiskinfo

The manifest installs the Windows package of the release, for x86_64 and for
arm64: `onyx` goes on the PATH, and OnyxDiskInfo goes in the Start menu.
Scoop checks the download against its SHA-256. Onyx reads most drives only
from a shell that runs as Administrator, and the app asks for it when it
starts. `scripts/scoop-manifest.sh` in the OnyxDiskInfo repository writes
`bucket/onyxdiskinfo.json` from the `SHA256SUMS` of each release.

## Where the manifest comes from

`scripts/scoop-manifest.sh` in the Burnout repository writes
`bucket/burnout.json` from the `SHA256SUMS` of each release. Change the
script, and not the manifest. A person writes each commit here. No bot pushes
to this bucket.

Report a problem in the
[issues of Burnout](https://github.com/Stiven-Gjekaj/burnout/issues).
