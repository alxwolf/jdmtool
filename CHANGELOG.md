# Changelog

## 0.5 (2025-08-08)
- Support for "older" Garmin USB Aviation Data Card Programmer devices (thanks [@alxwolf](https://github.com/alxwolf))
- Improvements to the `featunlk` script (thanks [@ELD400](https://github.com/ELD400) and [sHorst](https://github.com/sHorst))
- Display an error when trying to use an orange-label data card with a non-orange-label adapter
- Fix a crash when trying to update a read-only feat_unlk.dat file
- More Garmin devices are now officially supported

## 0.4.4.1 (2025-07-14)
- Unbreak the Skybound programmer device. Oops.

## 0.4.4 (2025-07-14)
- More features supported in `featunlk.dat` and a `featunlk` script for displaying various info
- Support for a few more data cards
- Very experimental, unfinished support for Terrain/Obstacles data cards
  - Does **not** support writing the databases yet; only raw bytes

Thank you [@ELD400](https://github.com/ELD400) and [sHorst](https://github.com/sHorst)!

## 0.4.3 (2025-05-04)
- Add support for the Avidyne IFD 400 "taildrm" feature
- Fix a few bugs with parsing of IFD 400 .dsf.txt files

## 0.4.2 (2025-02-12)
- Add an `extract-taw` command
- Allow downloading multiple services at once
- Retry when opening USB devices

## 0.4.1 (2025-01-23)
- Fix Garmin firmware not being included in the package
- Fix the FAT filesystem check on Windows

## 0.4.0 (2025-01-19)
- Add support for the Garmin Aviation Data Card Programmer
- Stop writing metadata to data cards
- Remove `read-metadata` and `write-metadata` commands
- Fix a bug causing negative volume IDs on Windows
- Require Python 3.9 or newer

## 0.3.6 (2025-01-07)
- Rewrite data card memory handling
- Properly support 2MB, 4MB, 8MB, and 16MB data cards
- Improve writing to data cards
- Add a "clear-card" command
- Add unit tests for data card logic

Thank you [@ELD400](https://github.com/ELD400) for all the help!

## 0.3.5 (2024-12-24)
- Support for Navdata for Avidyne EX5000
- Support for 8MB non-WAAS data cards for GNS 400/500 series
- Electronic Charts bug fixes

## 0.3.4 (2024-11-15)
- Fix an `Unsupported service category: '2'` error
- Fix a `LIBUSB_ERROR_NOT_SUPPORTED` error on Windows

## 0.3.3 (2024-10-10)
- Add support for orange 16MB WAAS cards (thanks [@bemowski](https://github.com/bemowski)!)
- Fix a crash when transferring G1000 basemaps
- Make libusb1 an optional dependency
- Remove libscrc dependency

## 0.3.2 (2024-08-12)
- Add a "clean" command
- Add --version
- Add shortcuts for transferring all current or all future versions

## 0.3.1 (2024-07-28)
- Fix the download location of grm_feat_key.zip
- Update docs

## 0.3 (2024-07-28)
- (Very experimental, possibly incomplete) Support for Garmin G1000 Electronic Charts
- Automatically download databases when transferring
- Transfer multiple databases at once
- A few UI improvements

## 0.2 (2024-06-04)
- (Very experimental) Support for Garmin G1000, except for Electronic Charts
- Optional JIT - improves transfer speed for IFD 400 and G1000

## 0.1 (2024-05-25)
- Support for Avidyne IFD 400 series
- Support for 4MB non-WAAS data cards for GNS 400/500 series
- Possibly fix accessing the Skybound device when it has an existing driver

## 0.0.4 (2024-04-12)
- Unbreak Python versions 3.7, 3.8, 3.9, 3.10

## 0.0.3 (2024-03-24)
- Fix refreshing services: the server started requiring the `cov_check` parameter
- Download sff files and keychain (though not used yet)
- Add a helper script for inspecting chartview files

## 0.0.2 (2023-04-10)
- Fix a crash when downloading files without crc32
- Improve UI

## 0.0.1 (2023-03-29)
- First release
- Supports programming GNS 430W
