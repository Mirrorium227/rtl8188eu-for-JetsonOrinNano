使用方式：
git clone https://github.com/Mirrorium227/rtl8188eu-for-JetsonOrinNano.git
sudo make -j$(nproc)
sudo make install
sudo modprobe 8188eu

原始编译日志：
jetson@yahboom:~/rtl8188eu$ sudo make -j$(nproc)
make ARCH=arm64 CROSS_COMPILE= -C /lib/modules/5.15.148-tegra/build M=/home/jetson/rtl8188eu  modules
make[1]: 进入目录“/usr/src/linux-headers-5.15.148-tegra-ubuntu22.04_aarch64/3rdparty/canonical/linux-jammy/kernel-source”
warning: the compiler differs from the one used to build the kernel
  The kernel was built by: gcc (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
  You are using:           gcc (Ubuntu 11.4.0-1ubuntu1~22.04.2) 11.4.0
  CC [M]  /home/jetson/rtl8188eu/rtw_cmd.o
  CC [M]  /home/jetson/rtl8188eu/rtw_security.o
  CC [M]  /home/jetson/rtl8188eu/rtw_debug.o
  CC [M]  /home/jetson/rtl8188eu/rtw_io.o
  CC [M]  /home/jetson/rtl8188eu/rtw_ioctl_query.o
  CC [M]  /home/jetson/rtl8188eu/rtw_ioctl_set.o
  CC [M]  /home/jetson/rtl8188eu/rtw_ieee80211.o
  CC [M]  /home/jetson/rtl8188eu/rtw_mlme.o
  CC [M]  /home/jetson/rtl8188eu/rtw_mlme_ext.o
  CC [M]  /home/jetson/rtl8188eu/rtw_mi.o
  CC [M]  /home/jetson/rtl8188eu/rtw_wlan_util.o
  CC [M]  /home/jetson/rtl8188eu/rtw_pwrctrl.o
  CC [M]  /home/jetson/rtl8188eu/rtw_rf.o
  CC [M]  /home/jetson/rtl8188eu/rtw_recv.o
  CC [M]  /home/jetson/rtl8188eu/rtw_sta_mgt.o
  CC [M]  /home/jetson/rtl8188eu/rtw_ap.o
  CC [M]  /home/jetson/rtl8188eu/rtw_xmit.o
  CC [M]  /home/jetson/rtl8188eu/rtw_p2p.o
  CC [M]  /home/jetson/rtl8188eu/rtw_tdls.o
  CC [M]  /home/jetson/rtl8188eu/rtw_br_ext.o
  CC [M]  /home/jetson/rtl8188eu/rtw_iol.o
  CC [M]  /home/jetson/rtl8188eu/rtw_sreset.o
  CC [M]  /home/jetson/rtl8188eu/rtw_btcoex_wifionly.o
  CC [M]  /home/jetson/rtl8188eu/rtw_btcoex.o
  CC [M]  /home/jetson/rtl8188eu/rtw_beamforming.o
  CC [M]  /home/jetson/rtl8188eu/rtw_odm.o
  CC [M]  /home/jetson/rtl8188eu/rtw_efuse.o
  CC [M]  /home/jetson/rtl8188eu/osdep_service.o
  CC [M]  /home/jetson/rtl8188eu/os_intfs.o
  CC [M]  /home/jetson/rtl8188eu/usb_intf.o
  CC [M]  /home/jetson/rtl8188eu/usb_ops2_linux.o
  CC [M]  /home/jetson/rtl8188eu/ioctl_linux.o
  CC [M]  /home/jetson/rtl8188eu/xmit_linux.o
  CC [M]  /home/jetson/rtl8188eu/mlme_linux.o
  CC [M]  /home/jetson/rtl8188eu/recv_linux.o
  CC [M]  /home/jetson/rtl8188eu/ioctl_cfg80211.o
  CC [M]  /home/jetson/rtl8188eu/rtw_cfgvendor.o
  CC [M]  /home/jetson/rtl8188eu/wifi_regd.o
  CC [M]  /home/jetson/rtl8188eu/rtw_android.o
  CC [M]  /home/jetson/rtl8188eu/rtw_proc.o
  CC [M]  /home/jetson/rtl8188eu/ioctl_mp.o
  CC [M]  /home/jetson/rtl8188eu/hal_intf.o
  CC [M]  /home/jetson/rtl8188eu/hal_com.o
  CC [M]  /home/jetson/rtl8188eu/hal_com_phycfg.o
  CC [M]  /home/jetson/rtl8188eu/hal_phy.o
  CC [M]  /home/jetson/rtl8188eu/hal_dm.o
  CC [M]  /home/jetson/rtl8188eu/hal_btcoex_wifionly.o
  CC [M]  /home/jetson/rtl8188eu/hal_btcoex.o
  CC [M]  /home/jetson/rtl8188eu/hal_mp.o
  CC [M]  /home/jetson/rtl8188eu/hal_mcc.o
  CC [M]  /home/jetson/rtl8188eu/hal_usb.o
  CC [M]  /home/jetson/rtl8188eu/hal_usb_led.o
  CC [M]  /home/jetson/rtl8188eu/HalPwrSeqCmd.o
  CC [M]  /home/jetson/rtl8188eu/Hal8188EPwrSeq.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_xmit.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_sreset.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_hal_init.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_phycfg.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_rf6052.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_dm.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_rxdesc.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188e_cmd.o
  CC [M]  /home/jetson/rtl8188eu/hal8188e_s_fw.o
  CC [M]  /home/jetson/rtl8188eu/hal8188e_t_fw.o
  CC [M]  /home/jetson/rtl8188eu/usb_halinit.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188eu_led.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188eu_xmit.o
  CC [M]  /home/jetson/rtl8188eu/rtl8188eu_recv.o
  CC [M]  /home/jetson/rtl8188eu/usb_ops_linux.o
  CC [M]  /home/jetson/rtl8188eu/HalEfuseMask8188E_USB.o
  CC [M]  /home/jetson/rtl8188eu/phydm_debug.o
  CC [M]  /home/jetson/rtl8188eu/phydm_antdiv.o
  CC [M]  /home/jetson/rtl8188eu/phydm_antdect.o
  CC [M]  /home/jetson/rtl8188eu/phydm_interface.o
  CC [M]  /home/jetson/rtl8188eu/phydm_hwconfig.o
  CC [M]  /home/jetson/rtl8188eu/phydm.o
  CC [M]  /home/jetson/rtl8188eu/halphyrf_ce.o
  CC [M]  /home/jetson/rtl8188eu/phydm_edcaturbocheck.o
  CC [M]  /home/jetson/rtl8188eu/phydm_dig.o
  CC [M]  /home/jetson/rtl8188eu/phydm_pathdiv.o
  CC [M]  /home/jetson/rtl8188eu/phydm_rainfo.o
  CC [M]  /home/jetson/rtl8188eu/phydm_dynamicbbpowersaving.o
  CC [M]  /home/jetson/rtl8188eu/phydm_powertracking_ce.o
  CC [M]  /home/jetson/rtl8188eu/phydm_dynamictxpower.o
  CC [M]  /home/jetson/rtl8188eu/phydm_adaptivity.o
  CC [M]  /home/jetson/rtl8188eu/phydm_cfotracking.o
  CC [M]  /home/jetson/rtl8188eu/phydm_noisemonitor.o
  CC [M]  /home/jetson/rtl8188eu/phydm_acs.o
  CC [M]  /home/jetson/rtl8188eu/phydm_dfs.o
  CC [M]  /home/jetson/rtl8188eu/phydm_hal_txbf_api.o
  CC [M]  /home/jetson/rtl8188eu/phydm_adc_sampling.o
  CC [M]  /home/jetson/rtl8188eu/phydm_kfree.o
  CC [M]  /home/jetson/rtl8188eu/phydm_ccx.o
  CC [M]  /home/jetson/rtl8188eu/halhwimg8188e_mac.o
  CC [M]  /home/jetson/rtl8188eu/halhwimg8188e_bb.o
  CC [M]  /home/jetson/rtl8188eu/halhwimg8188e_rf.o
  CC [M]  /home/jetson/rtl8188eu/halphyrf_8188e_ce.o
  CC [M]  /home/jetson/rtl8188eu/phydm_regconfig8188e.o
  CC [M]  /home/jetson/rtl8188eu/hal8188erateadaptive.o
  CC [M]  /home/jetson/rtl8188eu/phydm_rtl8188e.o
  CC [M]  /home/jetson/rtl8188eu/rtw_mp.o
  LD [M]  /home/jetson/rtl8188eu/8188eu.o
  MODPOST /home/jetson/rtl8188eu/Module.symvers
  CC [M]  /home/jetson/rtl8188eu/8188eu.mod.o
  LD [M]  /home/jetson/rtl8188eu/8188eu.ko
make[1]: 离开目录“/usr/src/linux-headers-5.15.148-tegra-ubuntu22.04_aarch64/3rdparty/canonical/linux-jammy/kernel-source”
jetson@yahboom:~/rtl8188eu$ sudo make install
install -p -m 644 8188eu.ko  /lib/modules/5.15.148-tegra/kernel/drivers/staging/r8188eu/
/sbin/depmod -a 5.15.148-tegra
jetson@yahboom:~/rtl8188eu$ sudo modprobe 8188eu
jetson@yahboom:~/rtl8188eu$ lsusb
Bus 002 Device 003: ID 2109:0817 VIA Labs, Inc. USB3.0 Hub
Bus 002 Device 002: ID 0bda:0411 Realtek Semiconductor Corp. Hub
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 011: ID 2109:8817 VIA Labs, Inc. USB Billboard Device
Bus 001 Device 010: ID 1a86:7523 QinHeng Electronics CH340 serial converter
Bus 001 Device 009: ID 0079:181c DragonRise Inc. Controller
Bus 001 Device 008: ID 10c4:ea60 Silicon Labs CP210x UART Bridge
Bus 001 Device 005: ID 2109:2817 VIA Labs, Inc. USB2.0 Hub
Bus 001 Device 007: ID 1a86:7522 QinHeng Electronics USB Serial
Bus 001 Device 006: ID 0d8c:0012 C-Media Electronics, Inc. USB Audio Device
Bus 001 Device 004: ID 1a86:8091 QinHeng Electronics USB HUB
Bus 001 Device 003: ID 0bda:0179 Realtek Semiconductor Corp. RTL8188ETV Wireless LAN 802.11n Network Adapter
Bus 001 Device 002: ID 0bda:5411 Realtek Semiconductor Corp. RTS5411 Hub
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
