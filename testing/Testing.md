# Test instructions

## Test 1 - mechanical test

- Success
  - Case assembles correctly
  - All connectors are snug with the case
- Failure
  - Top and bottom half of case are not aligned
  - Top and bottom half of case are not connected without a gap
  - C13/14 connectors do not fit without a gap

## Test 2 - Functionality test

- Setup
  - Connect the device to a mains supply
  - Connect the output to a C13 to plug socket adapter
  - Plug a raspberry pi in to the plug socket with its power adapter
  - Plug the relay into a linux device via usb
  - Ensure that the relay driver is installed on the host device: `sudo apt-get install usbrelay`
  - Run `sudo usbrelay PSUIS_1=1`

- Success
  - The Rpi powers on
- Failure
  - The Rpi doesn't power on

