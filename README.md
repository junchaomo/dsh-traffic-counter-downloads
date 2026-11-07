# DSH 车流量统计 · 官方下载

在 [Releases](https://github.com/junchaomo/dsh-traffic-counter-downloads/releases) 下载 Windows x64 安装包、对应源码和 SHA-256 校验文件。开发仓库保持私有，发布版对应源码依 AGPL-3.0 提供。

1. 安装 DeepSeek Harness 桌面版，解压完整安装包到固定目录。
2. 在解压目录打开 PowerShell，运行 `powershell -NoProfile -ExecutionPolicy Bypass -File .\install-windows.ps1`。
3. 打开 DSH → 车流量统计。若未出现侧栏入口，使用 DSH 的「添加插件」，选择解压目录里的 `dsh-traffic-counter` 子目录。

默认 CPU 推理使用 OpenVINO FP32。包内包含 Windows CPU 版 Python/PyTorch、YOLO26m 权重和动态 OpenVINO 模型。GPU 推理需要本机 NVIDIA 显卡、驱动以及与驱动匹配的 CUDA 版 PyTorch；CPU 安装包自身没有 CUDA 库。可在具备这些依赖的 Python 环境中运行 `web_app.py`。

本项目按 AGPL-3.0 发布；第三方组件保留各自许可证。源代码包提供构建脚本、导出脚本、安装脚本和应用源码。二进制包中的 runtime-versions.json 列出随附 Python 组件版本。Ultralytics 对应版本源码：https://github.com/ultralytics/ultralytics/tree/v8.4.189 。
