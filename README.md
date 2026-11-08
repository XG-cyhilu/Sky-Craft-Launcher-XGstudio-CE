# SCLCE · Sky Craft Launcher Community Edition

**SCL** is a minimalist launcher built with **Electron + React + Node.js + Vite**.

## Design Philosophy

> Minimal · Agile

## Features

1. Manage saves and resource packs for instances
2. In-depth server management with multi-server support
3. Agile window — resizes dynamically with the interface
4. Mouse-follow effect for a more organic window feel (can be disabled)
5. One-click switch between official and mirror sources
6. One-click mod downloads with automatic dependency resolution

## Acknowledgements

- [Electron](https://www.electronjs.org/), [React](https://react.dev/), [Vite](https://vite.dev/)
- [Fabric](https://fabricmc.net/), [Forge](https://files.minecraftforge.net/), [NeoForge](https://neoforged.net/), [Quilt](https://quiltmc.org/)
- [Modrinth](https://modrinth.com/) for its API and content
- [BMCLAPI](https://bmclapi2.bangbang93.com/) mirror
- [Azul Zulu](https://www.azul.com/downloads/), [Adoptium](https://adoptium.net/) for Java runtimes
- And all open-source projects and contributors this project depends on

## Development

### Clone

Official repository:

```bash
git clone https://github.com/SodiumMC/Sky-Craft-Launcher.git
cd Sky-Craft-Launcher
npm install
npm start
```

This repository:

```bash
git clone https://github.com/XG-cyhilu/Sky-Craft-Launcher-XGstudio-CE.git
cd Sky-Craft-Launcher-XGstudio-CE
pnpm install
pnpm start
```

### Scripts

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

## Gallery

<img width="300" height="225" alt="image" src="https://github.com/user-attachments/assets/e85a5e2f-4b27-4ca8-90a7-3a798e0657eb" />
<img width="300" height="192" alt="image" src="https://github.com/user-attachments/assets/ed3754d4-2c0e-4cbf-a718-2143984faa38" />
<img width="300" height="242" alt="image" src="https://github.com/user-attachments/assets/3cec3a44-1d5b-4d6b-8b3c-c5a2822ae77c" />
<img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/4681c592-6046-41b5-8063-05ccccc2fc55" />
<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/b1cc1bb8-7fbe-4af7-b83f-58a8e308a95e" />

## Copyright & License

| Project | Copyright | License |
| --- | --- | --- |
| SCLCE | Copyright © 2026 XG STUDIO | GNU GPLv3.0 |
| SCL | Copyright © 2026 OMS Work! | MIT |

## Disclaimer

Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.

**NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**
