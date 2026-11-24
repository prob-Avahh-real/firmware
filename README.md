# firmware

ESP32 嵌入式端侧 TensorFlow Lite Micro 模型常量与固件演示工程（已归档于 `archive/iot-firmware/firmware`）。

## 目录结构

- `esp32/main/model_demo.c`：端侧 TFLite Micro 量化模型字节数组（`g_demo_tflite_model`）C 源码示例
- `test/smoke.test.js`：固件目录与工程元数据完整性冒烟测试

## 目标平台（Target 判定）

- **移动端**：不适用（纯 ESP32 端侧嵌入式固件，无独立手机 App）
- **智能硬件**：需要（ESP32 微控制器端侧推理固件）

## 验证命令

```bash
npm test
```
