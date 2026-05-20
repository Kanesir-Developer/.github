<div align="center">

# Kanesir

**为下一代具身智能机器人提供软硬件平台**

[Website](https://kanesir.com) · [Contact](mailto:developer@kanesir.com)

</div>

### 关于我们

Kanesir 专注于商用服务机器人整机研发与云端运维平台,产品覆盖机器人本体、云控平台、移动端管理 App与开发者 SDK。

### 开发者 SDK

我们为 星驭 系列机器人提供官方SDK,开发者可以通过 SDK 订阅机器人状态、下发运动控制指令、触发紧急停止等核心能力。

| 仓库                                                                          | 语言   | 说明                   |
| ----------------------------------------------------------------------------- | ------ | ---------------------- |
| [karo-x2-sdk-python](https://github.com/Kanesir-Developer/karo-x2-sdk-python) | Python | 星驭X2 机型 Python SDK |
| [karo-x2-sdk-cpp](https://github.com/Kanesir-Developer/karo-x2-sdk-cpp)       | C++    | 星驭X2 机型 C++ SDK    |

### 快速开始

```bash
pip install karo-x2-sdk
```

```python
from karo_x2_sdk import RobotClient

client =RobotClient.connect("X2DP0100103000019")
client.state.subscribe(lambda s: print(s.pose))
client.cmd_vel(vx=0.2, vy=0.0, wz=0.0)
```
