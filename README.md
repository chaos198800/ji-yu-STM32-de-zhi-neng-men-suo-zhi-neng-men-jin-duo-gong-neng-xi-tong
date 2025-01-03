# 基于STM32的智能门锁/智能门禁多功能系统

## 项目简介

本项目是一个基于STM32F103C8T6微控制器的智能门锁/智能门禁多功能系统。该系统支持多种开锁方式，包括蓝牙、指纹识别、RFID刷卡和4x4键盘输入。系统设计灵活，界面友好，适用于家庭、办公室等多种场景。

## 主要功能

1. **蓝牙控制**：通过蓝牙模块进行远程控制，支持主管理员和副管理员权限设置。
2. **指纹识别**：使用AS608指纹模块进行指纹验证，支持指纹的添加和删除。
3. **RFID刷卡**：通过PN532 NFC RFID模块进行刷卡验证，支持多种类型的卡。
4. **4x4键盘输入**：通过4x4键盘进行密码输入，支持用户ID和密码认证。
5. **LCD显示**：使用TFT-ST7735S LCD屏幕提供友好的交互界面，显示系统状态和操作提示。

## 硬件模块

- **微控制器**：STM32F103C8T6
- **指纹模块**：AS608
- **RFID模块**：PN532 NFC RFID V3
- **蓝牙模块**：汇承HC-08
- **LCD显示**：TFT-ST7735S
- **电机驱动**：两路直流双H桥L298N
- **按键**：6*6*4轻触按键
- **下载器**：ST-LINK V2
- **电源**：DC12-3.3/5/7V
- **电池**：DC12-2800mAh

## 软件设计

- **数据存储**：使用闪存存储管理员、用户、指纹ID和卡号数据。
- **通信协议**：蓝牙、指纹、RFID刷卡使用USART，LCD使用SPI。
- **键盘扫描**：4x4键盘使用推挽输出和上拉输入进行扫描。

## 使用说明

1. **安装硬件**：按照电路图连接各硬件模块。
2. **烧录程序**：使用ST-LINK V2下载器将程序烧录到STM32F103C8T6芯片。
3. **配置系统**：通过蓝牙或键盘进行系统初始化和用户配置。
4. **使用系统**：根据需要选择指纹、RFID刷卡、蓝牙或键盘输入进行门锁控制。

## 注意事项

- 确保所有硬件连接正确，避免短路或接触不良。
- 在烧录程序前，确认芯片型号和内核版本，避免因内核差异导致的问题。
- 使用蓝牙模块时，需先进行测试和参数调整，确保通信稳定。

## 项目开源

本项目代码和相关资料已开源，欢迎开发者参与和改进。如有任何问题或建议，请在项目仓库中提交Issue或Pull Request。

---

通过本项目，您可以深入了解STM32微控制器的应用，掌握智能门锁系统的开发流程，并将其应用于实际生活中。希望本项目能为您的学习和开发提供帮助。

## 下载链接

[基于STM32的智能门锁智能门禁多功能系统](https://pan.quark.cn/s/a0ea632e9a41)