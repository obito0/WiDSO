# WiDSO
## 简介
通过Wi-Fi/USB显示和控制的数字示波器（DSO）/逻辑分析仪（LA）/信号发生器（DDS）等。  
由核心板（WiDSC）和扩展板两部分组成，最多可同时搭载两块扩展板。

### 核心板
- 通信接口：Wi-Fi b/g/n，USB FS，UART
- 扩展接口：两路，每路提供12个高速IO和4个ADC/PWM/SPI复用IO
- 存储空间：512k字节@16bits位宽
- 数据速率：采样/输出带宽之和最大100M字节/秒
- 调试方式：内建USB-Blaster和CDC串口，支持U盘方式升级
- 硬件组成：EPM240T100+IS61LV25616+STM32F103C8+ESP8266

### DSO扩展板（计划中）
- 通道数：1CH(8位)
- 采样率：100Mps Max
- 模拟带宽：>20MHz
- 输入幅度：+-4V(x1)/+-40V(x10) Max
- 触发方式：上升沿/下降沿，手动/单次/自动，支持触发信号输入/输出
- 硬件组成：ADC80100/AD9283-100，其余待定

### LA扩展板（计划中）
- 通道数：8CH
- 采样率：100Mps Max
- 输入电平：1.2~5.5V
- 逻辑触发：上升沿/下降沿/电平（任意通道组合），支持和DSO联合触发

### DDS扩展板（计划中）
- 通道数：1CH(8位)
- 采样率：100Mps Max
- 模拟带宽：>20MHz
- 输出幅度：+-4V Max，可调

### TFT扩展板（计划中）
- 分辨率：240*320
- 额外功能：Nor Flash/按键
