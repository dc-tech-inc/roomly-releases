# Roomly para Desktop — releases

Este repositorio existe **apenas para distribuir os instaladores** do Roomly
para Desktop. Ele nao contem codigo-fonte.

## Por que ele e separado

O aplicativo se atualiza sozinho usando o `update.electronjs.org`, que le a
release mais recente pela API publica do GitHub, sem autenticacao — ou seja,
ele exige um repositorio publico. E aqui que o Electron Forge publica os
artefatos de cada versao.

## Downloads

Os instaladores de cada versao estao em
[Releases](https://github.com/dc-tech-inc/roomly-releases/releases):

| Plataforma | Arquivo |
| --- | --- |
| Windows | `roomly-desktop-setup.exe` |
| macOS | `.dmg` |
| Linux | `.deb`, `.flatpak`, `.AppImage` |

## Licenca

O Roomly para Desktop e distribuido sob a **GNU Affero General Public License
v3.0**. E um fork de [`stoatchat/for-desktop`](https://github.com/stoatchat/for-desktop),
de Pawel Makles.
