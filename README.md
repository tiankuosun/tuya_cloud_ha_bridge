# Tuya-HA Connect

Tuya-HA Connect 是一个 Home Assistant 自定义集成，通过涂鸦 Tuya Link 协议将 HA 设备桥接到涂鸦云平台，实现双向控制。

## 功能

- 通过涂鸦 OpenAPI 自动创建虚拟网关设备
- 基于 MQTT (Tuya Link) 实现云端实时双向状态同步
- 支持品类：灯 (light)、开关 (switch)、风扇 (fan)、空调 (climate)、窗帘 (cover)、加湿器 (humidifier)、除湿器 (dehumidifier)、扫地机 (vacuum)、热水器 (water_heater)、媒体播放器 (media_player)、摄像头 (camera)
- 自动设备发现与绑定
- 支持涂鸦 App 远程控制 HA 设备

## 安装

### HACS 安装（推荐）

1. 在 HACS 中添加本仓库作为自定义仓库
2. 搜索 "Tuya-HA Connect" 并安装
3. 重启 Home Assistant

### 手动安装

1. 下载本仓库
2. 将文件复制到 `custom_components/tuya_cloud_ha_bridge/` 目录
3. 重启 Home Assistant

## 配置

1. 前往 **设置 > 设备与服务 > 添加集成**
2. 搜索 "Tuya-HA Connect"
3. 输入涂鸦云平台 API Key（从涂鸦开发者平台获取）
4. 按照提示完成配置

## 依赖

- Home Assistant 2024.1.0+
- paho-mqtt 2.1.0

## 许可证

[MIT License](LICENSE)
