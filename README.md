# bbbb-on-nixos

I am using a simple shell script that is run from a beaglebone black. The entire backup system
is fairly easy to setup. Just do a regular BBB install, clone the script repo, configure cron,
change the passwords and you're good.

Yet, I am wondering if it can still be easier with [Nixos](https://www.nixos.org). 

This repo contains my experiments.

https://nix.dev/tutorials/installing-nixos-on-a-raspberry-pi

https://github.com/zupo/nix/tree/further_simplification

First we're going to install nixos on a RPi, just to try it out.

Next we would want to make sure that all packages are installed that we need.

That'd be wake-on-lan, btrfs-tools, rsync and, of course, ssh.

  wget https://hydra.nixos.org/build/143434926/download/1/nixos-sd-image-20.09.4161.5b482ec815b-aarch64-linux.img.zst
  unzstd nixos-sd-image-20.09.4161.5b482ec815b-aarch64-linux.img.zst
  dd if=nixos-sd-image-20.09.4161.5b482ec815b-aarch64-linux.img.zst of=/dev/mmcblk0 status=progress

Check wifi



