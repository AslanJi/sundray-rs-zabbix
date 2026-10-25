# Sundray AS-Series Zabbix Template

Zabbix template for Sundray (信锐) AS-series access switches, based on SNMP.
Provides monitoring of interface status/traffic, CPU, memory, uptime, and device health.

## 项目简介

本项目为信锐安视（AS）系列交换机提供 Zabbix 监控模板，基于 SNMP 协议采集
端口状态与流量、CPU、运行时长及设备健康状态等指标。

## Features / 功能

- Interface status & traffic discovery (LLD) / 端口状态与流量自动发现
- Device uptime & sysinfo / 设备运行时长与系统信息
- Trigger templates for common alarms / 常用告警触发器模板

## Requirements / 环境要求

- Zabbix 8.0+ (tested) / 已在 Zabbix 6.0+ 测试
- SNMP v2c enabled on switches / 交换机需开启 SNMP v2c

## Usage / 使用方法

1. Import the template YAML into Zabbix / 将模板 YAML 导入 Zabbix
2. Link the template to your Sundray RS-series host / 将模板关联到信锐 AS 系列主机
3. Set the SNMP community macro `{$SNMP_COMMUNITY}` / 配置 SNMP 团体名宏

## License / 许可证

MIT
