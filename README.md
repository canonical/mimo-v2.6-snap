# MiMo V2.6 inference snap
[![mimo-v2-6](https://snapcraft.io/mimo-v2-6/badge.svg)](https://snapcraft.io/mimo-v2-6)



[MiMo-V2.6-Distill-Qwen-9B](https://huggingface.co/XiaomiMiMo/MiMo-V2.6-Distill-Qwen-9B) is a 9B multimodal agentic model developed by Xiaomi MiMo through supervised fine-tuning of Qwen3.5-9B on MiMo-generated data. It covers coding, general-purpose agent tasks, visual coding, and cybersecurity.

Use this snap to quickly install an optimized environment for local inference with MiMo V2.6.

The snap includes the following hardware-optimized inference engines:

* cpu: Optimized for x64 and ARM (armv8, armv9) CPUs
* nvidia-gpu: CUDA-enabled GPU acceleration

The most suitable engine is automatically selected based on the available hardware.

#### Install
```
sudo snap install mimo-v2-6
```

#### Run
```
mimo-v2-6
```

> [!TIP]
> Some accelerators require extra [drivers](https://documentation.ubuntu.com/inference-snaps/how-to/setup/drivers/) to be usable with this snap.

## Resources

📚 **[Documentation](https://documentation.ubuntu.com/inference-snaps/)**, learn how to use inference snaps

💬 **[Discussions](https://github.com/canonical/inference-snaps/discussions)**, ask questions and share ideas

🐛 **[Issues](https://github.com/canonical/inference-snaps/issues)**, report bugs and request features

## Build and install from source

Clone the repo:
```shell
git clone https://github.com/canonical/mimo-v2.6-snap
cd mimo-v2.6-snap
```

Initialize the development environment:
```shell
make init
```

Build and install snap:
```shell
make build
make install
```
