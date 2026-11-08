
# SCLCE · Sky Craft Launcher Community Edition

**SCL** 是一个使用 **Electron + React + Node.js + Vite** 的极简启动器。

## 设计理念

> 极简 · 灵动

## 特别功能

1. 管理实例的存档及资源包
2. 深度管理服务器，多服务器管理
3. 灵动窗口，窗口大小随界面动态变化
4. 鼠标跟随，窗口更优呼吸感（可关闭）
5. 官方源 / 镜像源 一键切换
6. 一键下载 mod，自动下载前置

## 开源项目致谢

- [Electron](https://www.electronjs.org/)、[React](https://react.dev/)、[Vite](https://vite.dev/)
- [Fabric](https://fabricmc.net/)、[Forge](https://files.minecraftforge.net/)、[NeoForge](https://neoforged.net/)、[Quilt](https://quiltmc.org/)
- [Modrinth](https://modrinth.com/) 提供的 API 与内容
- [BMCLAPI](https://bmclapi2.bangbang93.com/) 镜像
- [Azul Zulu](https://www.azul.com/downloads/)、[Adoptium](https://adoptium.net/) 提供的 Java 运行时
- 及本项目依赖的全部开源项目及其贡献者

## 开发
### 克隆
官方仓库
```bash
git clone https://github.com/SodiumMC/Sky-Craft-Launcher.git
cd Sky-Craft-Launcher
npm install
npm start
```

本仓库
```bash
git clone https://github.com/XG-cyhilu/Sky-Craft-Launcher-XGstudio-CE.git
cd Sky-Craft-Launcher-XGstudio-CE
pnpm install
pnpm start
```

### Script脚本
```json
  "scripts": {
    "build:main": "esbuild src/main/index.ts --bundle --platform=node --target=node20 --format=cjs --external:electron --outfile=dist/main/index.cjs",
    "build:preload": "esbuild src/preload/index.ts --bundle --platform=node --target=node20 --format=cjs --external:electron --outfile=dist/preload/index.cjs",
    "build:renderer": "vite build",
    "build": "npm run build:main && npm run build:preload && npm run build:renderer",
    "start": "node scripts/start.cjs",
    "typecheck": "tsc --noEmit",
    "test:ui": "node scripts/ui-test.mjs",
    "test:launch": "node scripts/launch-test.mjs",
    "package": "node scripts/package.mjs"
  }
```

## 画廊

<img width="300" height="225" alt="image" src="https://github.com/user-attachments/assets/e85a5e2f-4b27-4ca8-90a7-3a798e0657eb" />
<img width="300" height="192" alt="image" src="https://github.com/user-attachments/assets/ed3754d4-2c0e-4cbf-a718-2143984faa38" />
<img width="300" height="242" alt="image" src="https://github.com/user-attachments/assets/3cec3a44-1d5b-4d6b-8b3c-c5a2822ae77c" />
<img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/4681c592-6046-41b5-8063-05ccccc2fc55" />
<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/b1cc1bb8-7fbe-4af7-b83f-58a8e308a95e" />


## 版权与许可

| 项目 | 版权 | 许可 |
| --- | --- | --- |
| SCLCE | Copyright © 2026 XG STUDIO | GNU GPLv3.0 |
| SCL | Copyright © 2026 OMS Work! | MIT |

## 免责声明

非官方 Minecraft 产品，未经 MOJANG 或 MICROSOFT 批准或关联。

**NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**
