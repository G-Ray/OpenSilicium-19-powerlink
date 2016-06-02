# OpenSilicium-19-powerlink
Patch et defconfig à utiliser sur un Noyau 4.1 pour BeagleBone Black

```
git clone https://github.com/beagleboard/linux.git -b 4.1
cd linux
git reset --hard 71a2e76b837f57596ff185940221cb70f1ef914f
git revert 17cd5f95550aff7619ed4e2b2b0a0f9607d09431 #pour desactiver SMP
patch -p1 < 0001-Apply-patches-for-I-pipe-support-update-config.patch
```
