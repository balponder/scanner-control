# Scanner Control

A small web page for tracking warehouse equipment handouts (scanners, radios, other devices): who has which device, check-out and check-in history.

Live page: https://balponder.github.io/scanner-control/

## How it works
1. Scan the employee barcode, then the device barcode -> the device is checked out.
2. Scan only the device barcode -> the device is checked in.
3. Devices still out from previous days are shown as CARRYOVER.

Also includes employee management, device management (change type, correct barcode, remove/restore) and daily check-out / check-in history.

## Data and privacy
- No server, no database, no login. The page is one static HTML file (index.html).
- No data is sent over the internet. The page makes no network requests.
- Records are saved only on the local PC:
  - in the browser's own storage, and
  - in a folder the user chooses (Documents\Barcode Scanner Records): records.json, records.json.bak and Barcode_Scanner_Records.xlsx.
- The browser asks the user for permission before the page can write to that folder.
- This repository contains only the page code. It never contains employee or device data.

## Requirements
Microsoft Edge or Google Chrome. USB barcode scanners in keyboard mode work without any driver.

## Author
Burak Alponder
