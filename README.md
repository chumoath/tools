# tools

- e-pointer: http://foredu.com/
- pointfix: [language].ini -> pointofix_translation.ini

- windows如何查看usb设备的 bus dev func
  - 通过设备管理器/hwinfo/usbdeview/usbview 找到 port，bdf即为 1.[port].func，
  - rndis设备
    - func0通道为控制通道(URB_CONTROL 0x02)，获取描述符,发送控制信息
    - func1为数据通道(URB_BULK 0x03)，发送数据
    - func2为中断通道(URB_INTERRUPT 0x1)
                                                                                               
- usbdeview(nirsoft 一堆软件): https://www.nirsoft.net/, 绿色的圆点表示已连接的USB设备
- usbview (windows sdk): https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/
- siv: https://files2.majorgeeks.com/1bd403c7c108c3d33adf98737c19a823b7db1c77/systeminfo/siv_v5.82.zip
- HE: Hardware Read & Write Utility: https://github.com/Faintsnow/HE
- RW: https://rweverything.com/downloads/RwPortableX64V1.7.zip
- v2ray: https://github.com/v2ray/v2ray-core/releases
- sourcemonitor
- beyondcompare
- Mobaxterm
- vscode(remote ssh)
- sokit
- procexp64
- SETUNA
- ppgui
- wireshark
- pointofix
- sshfs winfsp
- vmware
- potplay
- git bash
- peview
- uefitool
- typora
- everything
- tcpview
- tftpd
- diskgenius
- notepad++
- EV录屏
- Perfect Backup
- Breeze
- Androi studio
- DBeaver
- DevEco Studio / devicetool
- powertoys
- TrafficMonitor
- JUDE / drawio / excalidraw / visio / 亿图图示


- rw everything rwdrv.sys 不能加载：
- 一、关闭“内存完整性”（必做）
此功能位于 Windows 安全中心内，是阻止未认证驱动加载的基础防护层：
打开 Windows 安全中心
按 Win + I → 进入 “隐私和安全性” → 选择 “Windows 安全中心” → 点击 “设备安全性”。
关闭“内存完整性”
进入 “内核隔离” → 关闭 “内存完整性” → 重启电脑234。

- 二、关闭“驱动阻止规则”（Driver Block Rules）（必做）
这是 Windows 11 22H2 新增机制，专门封禁如 RwDrv.sys 这类驱动：
修改注册表
按 Win + R → 输入 regedit → 回车（需管理员权限）。
定位路径并修改键值
导航到：
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\CI\Config
找到 VulnerableDriverBlocklistEnable → 双击将其值改为 0 → 重启

- JUDE
  - 修改 JUDE/jude.bat，将 路径修改为 JUDE的安装路径，set JUDE_HOME=D:\00-package\JUDE
  - jude.bat创建快捷方式，右键属性修改图标为 jude.ico
