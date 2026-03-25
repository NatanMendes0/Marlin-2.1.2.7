<p align="center"><img src="buildroot/share/pixmaps/logo/marlin-outrun-nf-500.png" height="250" alt="Logo do MarlinFirmware" /></p>

<h1 align="center">Firmware Marlin para Impressora 3D - Ender 3 Pro</h1>

<p align="center">
  <strong>Versão mais recente (até 25/03/2026) do firmware Marlin para Creality Ender 3 Pro (compilação STM32F103RE_creality)</strong>
</p>

Este repositório armazena a versão mais recente do firmware Marlin para minha **Creality Ender 3 Pro**, compilada para o microcontrolador **STM32F103RE_creality**.

## Sobre a Compilação

- **Impressora**: Creality Ender 3 Pro
- **Placa de Destino**: STM32F103RE_creality, v4.2.7
- **Firmware**: Firmware Marlin para Impressora 3D
- **Propósito**: Repositório pessoal de backup e configuração

Para documentação oficial do Marlin e suporte, visite a [Página Inicial do Marlin](//marlinfw.org/).

## Compilando e Carregando

Para compilar e carregar o Marlin, você usará uma destas ferramentas:

- O [Visual Studio Code](//code.visualstudio.com/download) gratuito usando a extensão [Auto Build Marlin](//marlinfw.org/docs/basics/auto_build_marlin.html).
- O [Arduino IDE](//www.arduino.cc/en/main/software) gratuito: Veja [Compilando Marlin com Arduino](//marlinfw.org/docs/basics/install_arduino.html)
- VSCode com devcontainer: Veja [Instalando Marlin (VSCode devcontainer)](http://marlinfw.org/docs/basics/install_devcontainer_vscode.html).

## Alterações de firmware aplicadas

A seguir, as diretivas que foram modificadas/ativadas na configuração:

- `#define USE_PROBE_FOR_Z_HOMING`
- `#define BLTOUCH`
- `#define NOZZLE_TO_PROBE_OFFSET { -55, -6, 0 }`
- `#define Z_PROBE_FEEDRATE_FAST (20*60)`
- `#define Z_CLEARANCE_DEPLOY_PROBE 6`
- `#define Z_CLEARANCE_BETWEEN_PROBES 3`
- `#define AUTO_BED_LEVELING_BILINEAR`
- `#define RESTORE_LEVELING_AFTER_G28`
- `#define Z_SAFE_HOMING`
- `#define GRID_MAX_POINTS_X 5`
- `#define BLTOUCH_DELAY 300`
- `#define BLTOUCH_HS_MODE true`
- `#define FWRETRACT`
- `#define BABYSTEP_MULTIPLICATOR_Z  0.01`
- `#define BABYSTEP_DISPLAY_TOTAL`
- `#define FWRETRACT`

Adicionalmente, o tamanho da mesa foi atualizado para:

- 180 x 220 x 200 (firmware + fatiador)

## Recursos

- [Documentação Marlin](//marlinfw.org)
- [Discord Marlin](//discord.com/servers/marlin-firmware-461605380783472640)
- [Configuração Marlin no YouTube](//www.youtube.com/results?search_query=marlin+configuration)

## Licença

Marlin é publicado sob a [licença GPL](/LICENSE).

