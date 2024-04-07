# A Kernel Seedling

This kernel module is intended to output the number of currently running processes on your system.

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