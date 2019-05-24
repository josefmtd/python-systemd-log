# python-systemd-log

This repository consists of example program to write logging info to systemd.
The systemd service calls the python program that will periodically report to systemd.

## Installing Dependencies

Under Debian/Ubuntu/Raspbian you can install the dependencies using aptitude.

```
# apt install build-essential
# apt install libystemd-dev
```

## Installing the Python Module

To install the Python3 systemd module, you can use pip3 or directly from aptitude.

```
# apt install python3-systemd
```

## Testing Python Log Service

Install the service by copying the pythonlog.service to `/lib/systemd/system/` and adding it to
systemd

```
# cp pythonlog.service /lib/systemd/system/pythonlog.service
# systemctl enable pythonlog.service
# systemctl start pythonlog.service
```
