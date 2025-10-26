# Switch 大气层整合包

## 根目录结构

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
| `bootloader/` | Hekate 引导加载器 | [Hekate 汉化](https://github.com/easyworld/hekate)   [Hekate 官方](https://github.com/CTCaer/hekate) |
| `config/` | 各类自制软件的配置文件 | 自动生成或手动配置 |
| `SaltySD/` | 底座插件的支持文件，包含一个系统模块 | [SaltyNX](https://github.com/masagrator/SaltyNX) |
| `switch/` | 自制软件存放目录 | 大气层标准目录 |
| `themes/` | 系统主题文件存放目录 | 手动创建 |
| `warmboot_mariko/` | Mariko 芯片专用的 warmboot 固件，用于从睡眠唤醒 | 大气层自动生成 |
| `exosphere.bin` | 8G 魔改文件，通过hekate引导进入 | [大气层 8G](https://github.com/TOM-BadEN/Atmosphere-mod) |
| `exosphere.ini` | 大气层配置文件，可以用来屏蔽序列号 | 大气层自带 |
| `hbmenu.nro` | Homebrew 菜单启动器，这里是sphaira | [sphaira（仓库停止更新）](https://github.com/ITotalJustice/sphaira)|
| `payload.bin` | 用于从系统内快速重启回 Hekate 菜单 | hekate.bin改名成payload.bin |

## atmosphere目录结构

```
atmosphere/
├── config/
├── contents/
├── exefs_patches/
├── hosts/
├── kips/
├── hbl.nsp
├── package3
├── reboot_payload.bin
└── stratosphere.romfs
```

| 目录/文件 | 说明 | 来源 |
|----------|------|------|
| `config/` | 大气层系统设置配置，包含 system_settings.ini 等系统级配置文件 | 大气层自动生成 |
| `contents/` | 系统模块存放目录，每个子目录对应一个 Title ID，包含模块文件和配置 | 各系统模块作者 |
| `exefs_patches/` | 系统补丁目录，用于修改系统功能，如 am 补丁、启动 logo 补丁等 | 补丁作者提供 |
| `hosts/` | DNS 劫持配置文件，包含默认、虚拟系统、真实系统的域名屏蔽列表 | 大气层自动生成 |
| `kips/` | KIP（Kernel Initial Process）加载器，包含 loader.kip 等核心进程 | 大气层核心组件 |
| `hbl.nsp` | Homebrew 启动器包，用于从相册等入口启动自制程序 | 大气层官方提供 |
| `package3` | 固件核心包，包含系统必需的组件 | 大气层核心组件 |
| `reboot_payload.bin` | 系统内重启时自动加载的 payload，通常指向 payload.bin | 大气层自动生成 |
| `stratosphere.romfs` | Stratosphere 层的资源文件系统，包含系统模块运行所需的资源 | 大气层核心组件 |