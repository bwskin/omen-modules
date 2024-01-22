# HP Omen 16 2022 (16-n0000) AMD modules

<a href='https://ko-fi.com/P5P4TQ3NM' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi3.png?v=3' border='0' alt='Buy Me a Coffee'/></a>

This repo contains linux kernel modules that fixes some issues with this model.

## How to install
```bash
git clone https://git.rustylab.net/public/omen-modules.git
cd omen-modules/<module-name>
sudo dkms install .
```

`<module-name>` is one of the follows:
- snd_hda_codec_realtek
- hp-wmi

# Special thanks to
- [Luis Bocanegra](https://github.com/luisbocanegra) - for giving me a good starting point and guideance at the beginning.
- [asus-linux.org](https://asus-linux.org) - for this [post](https://asus-linux.org/blog/sound-2021-01-11/). It gave me basic info on codecs, coeffs, etc.
- [joshua stein](https://jcs.org) - for his amazing [post](https://jcs.org/2018/11/12/vfio) about VFIO, Intel HDA and his [qemu patch](https://github.com/jcs/qemu/compare/e22f675b..jcs-hda-dma) which allowed me do log all neccesary data from drivers
- Tomas Espeleta - for [this patch](https://patchwork.kernel.org/project/alsa-devel/patch/20190114200353.4114-1-tomas.espeleta@gmail.com/). It was good example on how to write patches to realtek module
- @Lùmi - for bringing my attention to speaker channels mapping problem and motivation to finish audio fix
