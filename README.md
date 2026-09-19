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

### Releases y actualizaciones

El launcher se actualiza solo desde [GitHub Releases](https://github.com/Zergiv/ElDesvan/releases).

1. Sube la versión en `package.json` (p. ej. `1.0.1`).
2. Commit y push a `master`.
3. Crea y sube el tag: `git tag v1.0.1 && git push origin v1.0.1`
4. GitHub Actions publica los instaladores (`latest.yml`, `.exe`, `.dmg`, `.AppImage`).

El botón **Buscar actualizaciones** solo funciona en la app instalada (no con `pnpm start`).

### Créditos

Basado en [HeliosLauncher](https://github.com/dscalzi/HeliosLauncher) de Dscalzi.
