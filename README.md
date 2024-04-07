# A Kernel Seedling

This kernel module counts the number of currently running processes in the system and exposes this count via a virtual file named "count" in the /proc directory. When the /proc/count file is read, it outputs the total process count as a string. Upon loading (insmod), it logs an initialization message, and upon removal (rmmod), it logs an exit message and removes the /proc/count entry.

## Building
```shell
make
```

## Running
```shell
cat /proc/count
```
136

## Cleaning Up
```shell
make clean
```

## Testing
```python
python -m unittest
```

Passed all 3 tests

```shell
uname -r -s -v
```

Tested on Linux 5.14.8-arch1-1