# ESP Serial Find


[![pypi](https://img.shields.io/pypi/v/esp-serial-find.svg)](https://pypi.org/project/esp-serial-find/)
[![python](https://img.shields.io/pypi/pyversions/esp-serial-find.svg)](https://pypi.org/project/esp-serial-find/)
[![Build Status](https://github.com/ProfFan/esp-serial-find/actions/workflows/dev.yml/badge.svg)](https://github.com/ProfFan/esp-serial-find/actions/workflows/dev.yml)
[![codecov](https://codecov.io/gh/ProfFan/esp-serial-find/branch/main/graphs/badge.svg)](https://codecov.io/github/ProfFan/esp-serial-find)



Find the ESP32 serial port name with device serial number on macOS


* Documentation: <https://ProfFan.github.io/esp-serial-find>
* GitHub: <https://github.com/ProfFan/esp-serial-find>
* PyPI: <https://pypi.org/project/esp-serial-find/>
* Free software: MIT


## Features

* Find the ESP32 serial port name with device serial number on macOS
* `-s` option to print the path for the given serial number
* `-v` option to print verbose output
* Without any option: print all serial ports and their serial numbers

```bash
usage: esp-serial-find [-h] [--verbose] [--serial SERIAL]

options:
  -h, --help            show this help message and exit
  --verbose, -v         Print verbose output
  --serial SERIAL, -s SERIAL
                        Print the path for the given serial number
```

## Example

### Print all serial ports and their serial numbers

```bash
$ esp-serial-find
70:ee:50:1c:1b:0c /dev/cu.usbserial-0001
70:ee:50:1c:1b:0d /dev/cu.usbserial-0002
70:ee:50:1c:1b:0e /dev/cu.usbserial-0003
```

### Print the path for the given serial number

```bash
$ esp-serial-find -s 70:ee:50:1c:1b:0c
/dev/cu.usbserial-0001
```

## Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
