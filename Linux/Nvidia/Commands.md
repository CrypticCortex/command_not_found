### Using persistant mode 

The GPU state remains loaded in the driver whenever one or more clients have the device file open. Once all clients have closed the device file, the GPU state will be unloaded unless persistence mode is enabled.


``` sudo nvidia-smi -pm 0 ```

To turn it on

```sudo nvidia-smi -pm 1```
