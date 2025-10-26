# Switch 大气层整合包

## 目录结构

```
├── atmosphere/
├── bootloader/
├── config/
├── SaltySD/
├── switch/
├── themes/
├── warmboot_mariko/
├── exosphere.bin
├── exosphere.ini
├── hbmenu.nro
└── payload.bin
```

| 目录/文件 | 说明 | 来源 |
|----------|------|------|
| `atmosphere/` | 大气层核心文件夹 | [Atmosphere 官方](https://github.com/Atmosphere-NX/Atmosphere) |
| `bootloader/` | Hekate 引导加载器 | [Hekate 汉化](https://github.com/easyworld/hekate)，[Hekate 汉化](https://github.com/easyworld/hekate) |
| `config/` | 各类系统模块和自制软件的配置文件，包含 Ultrahand、Tesla、sys-clk、状态监控等工具配置 | 各工具自动生成或手动配置 |
| `SaltySD/` | SaltySD 游戏插件加载系统，包含插件文件、补丁和日志 | SaltySD 项目 |
| `switch/` | 自制软件和工具存放目录，包含 Ultrahand 工具包(.packages)、Tesla 插件(.overlays)、各类应用程序 | 各自制软件作者 |
| `themes/` | 系统主题文件存放目录，包含主题资源和补丁文件 | 主题作者制作 |
| `warmboot_mariko/` | Mariko 芯片专用的 warmboot 固件，用于从睡眠唤醒 | Atmosphere 官方提供 |
| `exosphere.bin` | Exosphere 安全监视器二进制文件 | Atmosphere 核心组件 |
| `exosphere.ini` | Exosphere 配置文件，可配置 8GB 内存支持等高级选项 | Atmosphere 配置文件 |
| `hbmenu.nro` | Homebrew 菜单启动器 | Atmosphere 官方提供 |
| `payload.bin` | 用于重启加载的 payload 文件 | Hekate 或其他 payload |
