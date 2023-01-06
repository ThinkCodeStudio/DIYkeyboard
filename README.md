 # DIYkeyboard

在键盘能使用的情况下使用串口终端?
85 key rgb lde 2ms delay 10ms

键盘下侧添加接口外接?

可二次开发， 内部编程的键盘

## 键盘布局

![layout](img/layout.png)

## 键盘拓扑模块

![module](img/a.png)

### 上侧模块

接口：
* USB 3.0 USB HUB
* GPIO
* SPI
* UART

硬件：
* USB 3.0接口
* 弹簧针触点

模块：
* GOIO开发拓扑
* USB HUB

### 左侧模块

接口：
* USB 3.0 USB HUB
* SPI
* UART

硬件：
* 弹簧针触点

模块：
* 智能旋钮
* USB HUB

### 下侧模块

接口：
* USB 3.0 USB HUB
* SPI
* UART

硬件：
* 弹簧针触点

模块：
* 触摸板
* USB HUB
* 外接电池

### 右侧模块

接口：
* USB 2.0 连接单片机
* SPI
* UART

硬件：
* 弹簧针触点

模块：
* 十六进制小键盘

## 键盘拓扑模块走线

![port](img/b.png)

## 硬件
* AT32F435ZMT7
* Flash W25Q128J
* SD卡
* 74HC165
* ST7789
* 磁轴?
* USB 3.0 HUB GL3520
* 编码器
* 拨码管 12pin*2
* 磁连接触点 (SPI&uart， 四个方向)
* 电池管理电路
* RTC电路
* RGB灯 WS2812
* usb type-c (偏右侧靠近芯片)
* 蓝牙模块 (暂时没有选型)
* 旋钮开关

## 驱动
* [ ] lcd
* [ ] 编码器
* [ ] 拨码管，使用IO拓展芯片扫描
* [ ] 按键扫描
* [ ] USB
* [ ] 蓝牙
* [ ] SD
* [ ] led

## 使用库
* rtthread
    * ulog
    * C++
    * ymodem
* eazyFlash
* pikaScript

## 功能

* [ ] bootloader
* [ ] HID协议
    * 鼠标和键盘通用?
    * USB HID
    * BLE HID
    * HID 媒体
* [ ] NKRO(全键无冲)
* [ ] Fn自定义快捷键
    * 读取文件自定义映射
    * 适配vim功能
    * 密码管理
* [ ] 轻量级运行时
    * 内存分配
    * 指令读取
    * 系统接口调用
* [ ] 内置计算器
* [ ] 电容触摸手势 *
* [ ] 文件配置读取
    * 键盘映射文件（编译过）
* [ ] 键盘一键启软件 *
* [ ] 电源管理
* [ ] 侧边拓扑模块接口
    * 扩展连接通信协议(四相通用)
* 按键录制

## 工具软件
* [ ] ~~脚本编译器~~
    * 前期终端编译
    * 后期QT图形界面
    * JSON结构
    * 编译运行脚本
    * 编译映射文件
    * 输出特定格式二进制文件





<!-- 尼尔，EVA ， 86 ，[ ] ，强尼， 凯  -->