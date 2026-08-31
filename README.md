# Roomly para Desktop — releases

Este repositorio existe **apenas para distribuir os instaladores** do Roomly
para Desktop. Ele nao contem codigo-fonte.

## Por que ele e separado

O aplicativo se atualiza sozinho usando o `update.electronjs.org`, que le a
release mais recente pela API publica do GitHub, sem autenticacao — ou seja,
ele exige um repositorio publico. E aqui que os artefatos de cada versao sao
publicados.

## Downloads

Tudo em [Releases](https://github.com/dc-tech-inc/roomly-releases/releases).

| Plataforma | Arquivo |
| --- | --- |
| Windows | `roomly-desktop-setup.exe` |
| macOS (Apple Silicon) | `Roomly-<versao>-arm64.dmg` |
| macOS (Intel) | `Roomly-<versao>-x64.dmg` |
| Linux — universal | `Roomly-<versao>-anylinux-x86_64.AppImage` (ou `aarch64`) |
| Linux — Debian/Ubuntu | `roomly-desktop_<versao>_amd64.deb` (ou `arm64`) |
| Linux — Flatpak | `life.roomly.RoomlyDesktop_stable_x86_64.flatpak` (ou `aarch64`) |

Os `.zip` de cada plataforma e os arquivos `RELEASES`, `.nupkg` e `.zsync`
sao usados pelo mecanismo de atualizacao automatica; para instalar, use os da
tabela acima.

> **Nota:** os binarios ainda **nao sao assinados**. No Windows o SmartScreen
> mostra "aplicativo nao reconhecido"; no macOS, abra pelo menu de contexto
> (botao direito > Abrir) na primeira vez.

## Licenca

O Roomly para Desktop e distribuido sob a **GNU Affero General Public License
v3.0**. E um fork de [`stoatchat/for-desktop`](https://github.com/stoatchat/for-desktop),
de Pawel Makles.
