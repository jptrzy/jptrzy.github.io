---
title: "Small librebooted x60s journey"
date: 2022-11-09T23:21:15+01:00
---

Since I start using my X220 I always wanted to install libreboot on it.
Unfortunately for me libreboot [never came for it](https://libreboot.org/docs/hardware/) and I was left with coreboot.
But because I have a long list of things to do I never have time to even touch it.

So years go by and I had finally forgotten about it.
Then one week ago when I was searching (for some unknown reason) for x60 I found a really good offer for it.
One advantage of the offer was that it was librebooted from the start and that I needn't install it (Yes, I know that it is easy to install it on x60).
So I bought it and ...

## Libreboot

... when I get it my small amount of knowledge and understanding of libreboot documentation take the direction of the story.
Firstly laptop comes without a hard drive, so I put in an old 60G drive with alpine linux installed on it.
After a few unsuccessful attempts to boot it, I install grub on it and everything starts working fine.

It appears that libreboot has build-in grub and all you need is to generate `/boot/grub/grub.cfg` by running `grub-mkconfig -o /boot/grub/grub.cfg`.

Another problem I come by was its unwillingness to work with some pen drives.
Usually, I just needed to plug it out and in, but sometimes it wouldn't help and the only help was in grub console mode *(or just it didn't work)*.

## Parabola linux

I like alpine linux, but I wanted to have something with 100% free software and it wasn't visible with alpine, so I tried installing [parabola linux](https://www.parabola.nu/).

The first problem was that I couldn't boot it for [some](https://labs.parabola.nu/issues/2108) reason, but when I booted [the old iso](https://mirrors.dotsrc.org/parabola/iso/parabola-openrc-2021.08.11/parabola-openrc-2021.08.11-dual.iso) of it and [dealt](https://wiki.manjaro.org/index.php/Pacman_troubleshooting#Errors_about_Keys) with some outdated pgp keys everything went fine. *(It was a mess.)*

After installation most things went just fine, I rebooted the system and maybe forgot about installing some basic openrc packages, but after burning more time I have quite a usable system.

*If you would think about installing parabola linux firstly you can convert your current archlinux system (if you have one) into parabola one and secondly you might want to think about installing `your-freedom` and `your-privacy` packages.*

### Software

The next obstacle on my way to a usable daily driver was unwillingness of some software to work well.

One of which was firefox that I replaced for [vimb](https://fanglingsu.github.io/vimb). Why not [surf](https://surf.suckless.org/) someone could ask; for some reason it is slower than vimb or [qutebrowser](https://www.qutebrowser.org/).

## Plans for the future

One of the annoyances of x60 for me is its screen low brightness. So I'm thinking about doing "small" mod that I found is [possible](https://youtu.be/coJdBNazXuA?t=200).

Use express card slot for [something](https://www.youtube.com/watch?v=fYvozIP58Vo) fun or [useful](https://thinkmods.store/collections/all-mods-1/products/expresscard-to-nvme-adapter).
