# GPU Acceleration Guide

1. Install python 3.9.x or 3.10.x (recommended [3.10.11](https://www.python.org/downloads/release/python-31011/) bc it worked for me)
2. Make virtual environment using `venv` 
    1. creating `venv 
    python3.10 -m venv .venv`
    or
    `python3.9 -m venv .venv` 
    2. activate `venv` 
    `source ./.venv/bin/activate`
        1. Check the version using `python --version`
    3. install `pip` 
    `python -m pip install -U pip` 
3. Install `tensorflow` 
    1. `python -m pip install tensorflow tensorflow-macos tensorflow-metal` 
4. Verification
    1. Use the `Untitled.ipynb` file.
5. If it’s not working

If the first cell doesn’t return the output below, you may have to remake the environment.

```
TensorFlow has access to the following devices:
[PhysicalDevice(name='/physical_device:CPU:0', device_type='CPU'), PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]
TensorFlow version: 2.16.2
```

1. Remove the original environment
`sudo rm -rf .venv` 
2. Go back to `2.` 

References

https://heytech.tistory.com/295

https://developer.apple.com/metal/tensorflow-plugin/
