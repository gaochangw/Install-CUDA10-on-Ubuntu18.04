# CUDA 10 Installation Guide on Ubuntu 18.04

## Install GPU Driver:
```
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt install nvidia-driver-415
reboot
```
After reboot check if the driver is installed properly by:
```
nvidia-smi
```

## Install CUDA 10 using runfile:
```
chmod +x ./cuda_10.0.130_410.48_linux.run
./cuda_10.0.130_410.48_linux.run --extract=$HOME
~/.cuda-linux.10.0.130-24817639.run
echo 'export CUDA_HOME=/usr/local/cuda' > ~/.bashrc
echo 'export PATH=/usr/local/cuda/bin:$PATH'
```


