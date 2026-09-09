<img src="icon-256.png" width="96" align="right" alt="">

# Baixar o Roomly para computador

Este repositório serve **só para hospedar os arquivos de instalação**. Não tem
código aqui.

### → [**Clique aqui para baixar a versão mais recente**](https://github.com/dc-tech-inc/roomly-releases/releases/latest)

Na página que abrir, procure a seção **Assets** e escolha o arquivo do seu
sistema, usando a tabela abaixo.

---

## Qual arquivo eu baixo?

### 🪟 Windows

**Baixe `roomly-desktop-setup.exe`.** É só isso — um arquivo, clique duplo,
pronto. Serve para Windows 10 e 11.

### 🍎 Mac

Depende do processador do seu Mac. Para descobrir em 5 segundos:

> Clique na 🍎 no canto superior esquerdo → **Sobre este Mac**.
> Se aparecer **Apple M1, M2, M3** ou similar, é Apple Silicon.
> Se aparecer **Intel**, é Intel.

| Seu Mac | Arquivo |
| --- | --- |
| Apple Silicon (M1/M2/M3/M4) | `Roomly-<versão>-arm64.dmg` |
| Intel | `Roomly-<versão>-x64.dmg` |

Na dúvida entre os dois: Macs vendidos a partir de **2021** são quase sempre
Apple Silicon.

### 🐧 Linux

Se você não faz ideia de qual escolher, **baixe o `.AppImage`** — ele funciona
em qualquer distribuição, não precisa instalar nada, é só dar permissão de
execução e abrir.

| Como você prefere instalar | Arquivo |
| --- | --- |
| **Não sei / qualquer distro** | `Roomly-<versão>-anylinux-x86_64.AppImage` |
| Ubuntu, Debian, Mint, Pop!_OS | `roomly-desktop_<versão>_amd64.deb` |
| Fedora, ou quem já usa Flatpak | `life.roomly.RoomlyDesktop_stable_x86_64.flatpak` |

Nos três casos, se o seu computador for **ARM** (Raspberry Pi, alguns
notebooks novos), troque `x86_64` por `aarch64` e `amd64` por `arm64`. Se você
não sabe o que é isso, é porque não é o seu caso — use a versão normal.

---

## "O Windows/Mac disse que o arquivo é perigoso"

**Isso é esperado e o Roomly não é um vírus.** Os instaladores ainda não têm
assinatura digital — que é um certificado pago que diz ao sistema quem
publicou o programa. Sem ele, Windows e macOS avisam sobre qualquer programa,
inclusive os legítimos.

**No Windows**, vai aparecer uma tela azul do *SmartScreen* dizendo
"O Windows protegeu o computador":

1. Clique em **Mais informações**
2. Clique em **Executar assim mesmo**

**No Mac**, vai dizer que o app "não pôde ser aberto porque é de um
desenvolvedor não identificado":

1. **Não** dê dois cliques no app
2. Clique nele com o **botão direito** → **Abrir**
3. Na caixa que aparecer, clique em **Abrir** de novo

Só é preciso fazer isso **na primeira vez**. Depois abre normal.

---

## Perguntas rápidas

**Preciso baixar de novo quando sair versão nova?**
Não. O Roomly se atualiza sozinho.

**E aqueles outros arquivos na lista?**
Os `RELEASES`, `.nupkg`, `.zsync` e `.zip` são usados pela atualização
automática. Você não precisa baixar nenhum deles.

**Quanto ocupa?**
Entre 85 MB e 135 MB, dependendo da plataforma.

**Não tenho como instalar nada nesta máquina.**
O Roomly funciona no navegador, sem instalar: **https://roomly.life/app**

---

## Detalhes técnicos

O aplicativo se atualiza pelo `update.electronjs.org`, que lê a release mais
recente pela API pública do GitHub, sem autenticação — por isso este
repositório é público e separado do código.

O Roomly para Desktop é distribuído sob a **GNU Affero General Public License
v3.0**. É um fork de
[`stoatchat/for-desktop`](https://github.com/stoatchat/for-desktop), de Pawel
Makles. O código-fonte está em
[`dc-tech-inc/roomly-desktop`](https://github.com/dc-tech-inc/roomly-desktop).
