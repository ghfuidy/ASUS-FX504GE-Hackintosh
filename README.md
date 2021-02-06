# OpenCore EFI (0.6.4) for FX504GE FX80G

## Abstract:

Some modifies have been made. Update OC version to 0.6.4 according to the previous EFI（https://github.com/PoomSmart/ASUS-FX504GE-Hackintosh）. This EFI modified config.plist, change drivers and add some new kext plugins.

## Notes:



| Parameters  | Configuration                                                |
| ----------- | ------------------------------------------------------------ |
| CPU         | intel-8300H                                                  |
| motherboard | ASUSTeK COMPUTER INC. FX504GE (Coffee Lake)                  |
| memory      | 16G ( add an other 8G RAM)                                   |
| storage     | 500G Nvme ( WD SN550, new hard disk repurchased to install MacOS) |

## BIOS Settings:

1. VT-d: Disabled
2. Secure Boot: Disabled
3. Fast-Boot: Disabled
4. SATA mode: AHCI
5. DVMT-Preallocated: 64MB



## Important：

To disable CFG-LOCK，option `AppleCpuPmCfgLock` and `AppleXcpmCfgLock` under `Kernel -> Quirks` were opened.

Better solution for off CFG-LOCK is in this web: https://dortania.github.io/OpenCore-Post-Install/misc/msr-lock.html#checking-if-your-firmware-supports-cfg-lock-unlocking



**中文说明：OC的EFI可直接替换安装镜像中的EFI或在安装镜像中新建分区放置OC的EFI文件，作为安装启动使用，安装完毕后，将没有问题的EFI拖入系统EFI分区中作为引导使用。** 

