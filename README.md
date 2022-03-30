# Lenovo-ThinkStation-P310-Hackintosh
联想ThinkStation P310 黑苹果驱动

| 规格     | 详细信息                                     |
| -------- | -------------------------------------------- |
| 电脑型号 | 联想ThinkStation P310                           |
| 处理器   | 英特尔 酷睿 i5-6500                         |
| 硬盘     | Kingston A400        |
| 显卡     | Intel HD Graphics 530 |  NVIDIA Quadro K420
| 内存     | 16 GB DDR4                                 |
| 显示器   | 联想配套显示器 x 1                    |
| 声卡     | Realtek ALC662 板载                              |
| 有线网卡 | Intel 1219-LM2 板载                             |


## 注意事项
- [ ] **只能使用主机自带的两个DP接口的下方那个DP输出，或者使用板载VGA输出**
- [ ] **BIOS修改显示设置为板载显卡，分配内存修改为64M，不可使用独显输出**
- [ ] **BIOS的串形端口菜单中关闭串口**
- [ ] **使用UEFI启动**

## 驱动情况
- [x] HD 530核显驱动正常，独显屏蔽
- [x] USB驱动正常
- [x] 声音输出正常

## 独显驱动问题
- [ ] 独显也是可以驱动的，显卡设置改成Auto
- [ ] 修改config中的-Misc➡SecureBootMode➡Disable和NVRAM➡7C436110-AB2A-4BBB-A880-FE41995C9F82➡csr-active-config ➡ EF0F0000
- [ ] 终端执行命令：sudo spctl --master-disable
- [ ] 重启到Recovery，执行csrutil disable 关闭SIP
- [ ] 重启执行reset nvram
- [ ] 按照这个项目安装驱动，https://github.com/chris1111/Geforce-Kepler-patcher
- [ ] 具体教程自行搜索

## 已知问题
- [ ] **查看Releases页详细说明**

## 更新日志

### 2022年3月10日 Monterey 12.2.1 OpenCore 0.7.8

## 成品EFI查看Releases
