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
