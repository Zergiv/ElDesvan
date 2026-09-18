<p align="center"><img src="./app/assets/images/SealCircle.png" width="150px" height="150px" alt="El Desván"></p>

<h1 align="center">El Desván ✨</h1>

<em><h5 align="center">Launcher basado en Helios Launcher</h5></em>

[<p align="center"><img src="https://img.shields.io/github/actions/workflow/status/Zergiv/ElDesvan/build.yml?branch=master&style=for-the-badge" alt="gh actions">](https://github.com/Zergiv/ElDesvan/actions) [<img src="https://img.shields.io/github/downloads/Zergiv/ElDesvan/total.svg?style=for-the-badge" alt="downloads">](https://github.com/Zergiv/ElDesvan/releases)</p>

<p align="center">Únete al servidor sin preocuparte de instalar Java, Forge u otros mods. Nosotros nos encargamos.</p>

## Características

* Gestión completa de cuentas (Microsoft + Mojang).
* Gestión eficiente de assets y validación de archivos.
* Validación e instalación automática de Java.
* Feed de noticias integrado.
* Ajustes intuitivos, incluyendo panel de control de Java.
* Actualizaciones automáticas del launcher.

## Descargas

Desde [GitHub Releases](https://github.com/Zergiv/ElDesvan/releases)

| Plataforma | Archivo |
| -------- | ---- |
| Windows x64 | `ElDesvan-setup-VERSION.exe` |
| macOS x64 | `ElDesvan-setup-VERSION-x64.dmg` |
| macOS arm64 | `ElDesvan-setup-VERSION-arm64.dmg` |
| Linux x64 | `ElDesvan-setup-VERSION.AppImage` |

## Consola

```console
ctrl + shift + i
```

## Desarrollo

**Requisitos:** [Node.js](https://nodejs.org/en/) v22 y [pnpm](https://pnpm.io/)

```console
> git clone https://github.com/Zergiv/ElDesvan.git
> cd ElDesvan
> pnpm install
> pnpm start
```

**Build**

```console
> pnpm run dist
```

| Plataforma    | Comando              |
| -------- | ---- |
| Windows x64 | `pnpm run dist:win`   |
| macOS       | `pnpm run dist:mac`   |
| Linux x64 | `pnpm run dist:linux` |

### Configuración pendiente

Antes de lanzar en producción, configura:

1. **Distribution URL** en `app/assets/js/distromanager.js` (`REMOTE_DISTRO_URL`) — apunta al `distribution.json` de tu servidor (Nebula).
2. **Enlaces sociales** en `app/assets/lang/_custom.toml` (Discord, YouTube, etc.).
3. **Microsoft Auth** si necesitas un Client ID propio — ver [docs/MicrosoftAuth.md](docs/MicrosoftAuth.md).

### Créditos

Basado en [HeliosLauncher](https://github.com/dscalzi/HeliosLauncher) de Dscalzi.
