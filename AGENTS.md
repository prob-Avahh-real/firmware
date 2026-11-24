# firmware

固件 / BLE / MQTT 相关（已归档）

## 用途与 Target 判定

固件 / BLE / MQTT 相关（已归档）

- 移动端：不适用（纯 ESP32 嵌入式端侧模型固件）
- 智能硬件：需要

## 目标平台

| 平台 | 方式 | 产出 |
|------|------|------|
| 移动端 | 不适用 | 纯 ESP32 固件，无独立 App |
| 智能硬件 | 需要 | ESP32 端侧 TFLite 模型固件 |

## 命令

```bash
# 见 README；归档工程以只读/小修为主
```

## 状态

已归档。默认只做必要修复与知识库同步，不新开大范围需求。

## 智能硬件约定

- 戒指：DeviceOrientation；手杖：DeviceMotion；手表窄屏 CSS
- 复用 shared / 兄弟项目模块，避免复制漂移

## 助手约束

- Loop：先定可验证 Done 与停止条件；每切片过验证环；失败回灌；详见 docs/LOOP_ENGINEERING.md
- Harness：遵循根 AGENTS「Harness Engineering」；Guide=本文件，Sensor=测试/CI；同类失误二次须沉淀规则或测试（棘轮）。详见 docs/HARNESS_ENGINEERING.md
- 遵循仓库根 `/Users/skat/AGENTS.md` 与本文件的用途判定
- 可选 Target 可搁置；不适用形态不要硬加
- 改动聚焦；公共逻辑抽离复用
