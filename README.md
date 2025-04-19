# 🐉 Skyrim Modding Essentials - Guia Essencial PT-BR

**Nota:** Guia focado nos passos e mods **absolutamente essenciais** para uma base de modding estável e funcional em Português do Brasil.
*Atualizado com práticas recomendadas.*

---

## 📜 Índice
1. [**Qual Versão do Skyrim Comprar? (SE vs AE)**](#-qual-versão-do-skyrim-comprar-se-vs-ae)
2. [**Instalação Limpa do Jogo (Steam)**](#-instalação-limpa-do-jogo-steam)
3. [**Ferramentas Essenciais de Modding**](#-ferramentas-essenciais-de-modding)
4. [**Configurando as Ferramentas (SKSE, MO2, LOOT)**](#-configurando-as-ferramentas-skse-mo2-loot)
5. [**Configuração PT-BR (Legendas + Dublagem)**](#-configuração-pt-br-legendas--dublagem)
6. [**Mods FUNDAMENTAIS (Base Obrigatória)**](#-mods-fundamentais-base-obrigatória)
7. [**FAQ e Solução de Problemas Comuns**](#-faq-e-solução-de-problemas-comuns)

---

## 🛒 Qual Versão do Skyrim Comprar? (SE vs AE)

| Versão                   | Link de Compra                                          | Recomendação para Modding                                                                                                                                                           |
| :----------------------- | :------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Special Edition (SE)** | [Steam](https://store.steampowered.com/app/489830)      | **Recomendada para iniciar.** Versão base 64-bit com as 3 DLCs oficiais. Maior estabilidade histórica com mods que usam SKSE.                                                     |
| **Anniversary Edition (AE)** | [Upgrade na Steam](https://store.steampowered.com/app/1746860) | SE + todo conteúdo Creation Club. Funciona bem, mas atualizações da Bethesda podem quebrar SKSE temporariamente, exigindo espera por updates ou uso do Downgrade Patcher. |

**Conclusão:** Comece com a **Special Edition (SE)** para maior simplicidade. Se já tiver a AE ou quiser o conteúdo extra, esteja ciente da necessidade potencial de gerenciar versões do jogo/SKSE, especialmente após atualizações do jogo. Muitos usam o [Downgrade Patcher](https://www.nexusmods.com/skyrimspecialedition/mods/57618) na AE para máxima compatibilidade com mods SKSE.

---

## 🖥️ Instalação Limpa do Jogo (Steam)

1.  **Compre e Instale o Skyrim SE** no Steam.
2.  **Local de Instalação:** **NÃO instale** dentro de `C:\Program Files` ou `C:\Program Files (x86)`. Crie uma pasta separada (ex: `C:\Games\SteamLibrary`) e adicione-a como biblioteca no Steam (`Steam > Configurações > Downloads > Pastas de Biblioteca Steam`). Instale o Skyrim lá.
3.  **Primeira Execução:** Inicie o Skyrim SE pelo launcher do Steam **uma vez**. Deixe detectar o hardware e criar os arquivos `.ini` (`Documentos\My Games\Skyrim Special Edition`). Pode fechar na tela inicial.

---

## 🛠️ Ferramentas Essenciais de Modding

Estas são **obrigatórias**.

| Ferramenta                             | Download                                                                                              | Função Essencial                                                       |
| :------------------------------------- | :---------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------- |
| **Mod Organizer 2 (MO2)**              | [Nexus Mods](https://www.nexusmods.com/skyrimspecialedition/mods/6194)                                | Gerenciador de mods indispensável (isola mods do jogo original).      |
| **Skyrim Script Extender (SKSE64)**    | [Site Oficial](https://skse.silverlock.org/)                                                           | Permite que mods complexos funcionem (necessário para SkyUI e muitos outros). |
| **LOOT (Load Order Optimisation Tool)** | [Site Oficial](https://loot.github.io/)                                                               | Organiza a ordem de carregamento dos mods para evitar conflitos.       |

---

## ⚙️ Configurando as Ferramentas (SKSE, MO2, LOOT)

1.  **Instale o SKSE64:**
    *   Baixe a versão correspondente à sua versão do Skyrim (SE ou AE) no [Site Oficial](https://skse.silverlock.org/).
    *   Extraia o `.7z` baixado.
    *   Copie os arquivos `.dll` e `.exe` para a pasta raiz do Skyrim SE (onde fica `SkyrimSE.exe`, ex: `C:\Games\SteamLibrary\steamapps\common\Skyrim Special Edition`).
    *   Copie a pasta `Data` do arquivo extraído para dentro da pasta `Data` do Skyrim SE (mescle se perguntar).
    *   **IMPORTANTE:** A partir de agora, **SEMPRE** inicie o Skyrim pelo `skse64_loader.exe` (faremos isso via MO2).

2.  **Instale e Configure o Mod Organizer 2 (MO2):**
    *   Instale o MO2 ([Nexus Link](https://www.nexusmods.com/skyrimspecialedition/mods/6194)). Prefira a instalação "Portátil" (Portable).
    *   Abra o MO2. Selecione "Skyrim Special Edition". Confirme o caminho do jogo. Autorize a conexão com o Nexus Mods se perguntar.
    *   **Adicione o SKSE no MO2:** Clique nas engrenagens (🔧) > No campo "Executável", clique em `<Edit...>` > Clique no `+` > "Adicionar de Arquivo..." > Navegue até a pasta raiz do Skyrim e selecione `skse64_loader.exe`. Dê um nome (ex: "SKSE") > Clique "Aplicar" e "OK".
    *   **Sempre deixe "SKSE" selecionado no menu dropdown de execução** antes de clicar em "Executar" para jogar.

3.  **Adicione o LOOT no MO2:**
    *   Instale o LOOT ([Site Oficial](https://loot.github.io/)).
    *   No MO2, clique nas engrenagens (🔧) > `+` > "Adicionar de Arquivo..." > Navegue até onde instalou o LOOT e selecione `LOOT.exe`. Clique "Aplicar" e "OK".
    *   Para organizar seus mods, selecione "LOOT" no dropdown do MO2 e clique "Executar". Dentro do LOOT, clique em "Sort Plugins" (ícone de 3 linhas) e depois em "Apply". Feche o LOOT. **Faça isso sempre que instalar/remover mods com plugins (.esp/.esm).**

---

## 🇧🇷 Configuração PT-BR (Legendas + Dublagem)

1.  **Legendas PT-BR (Oficial Steam):**
    *   Biblioteca Steam > Botão direito no Skyrim SE > Propriedades > Idioma > Selecione "Português - Brasil". O Steam baixará os arquivos necessários.

2.  **Dublagem PT-BR (Mod da Comunidade):**
    *   **Skyrim Special Edition Dublado PT-BR:** [Procurar no Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/54591) (Verifique o link mais recente no Nexus).
    *   Baixe o arquivo principal pelo MO2 (ou manualmente e adicione via ícone 📦 no MO2).
    *   Ative o mod no painel esquerdo do MO2. Certifique-se que o plugin `.esp` da dublagem está ativado no painel direito (aba "Plugins"). Execute o LOOT depois de instalar.

---

## 🛠️ Mods FUNDAMENTAIS (Base Obrigatória)

Estes mods formam a base essencial para qualquer setup. Instale **todos** via MO2 e execute o LOOT após instalar.

| Mod                                     | Descrição                                                                      | Link                                                                    | Notas / Dependências         |
| :-------------------------------------- | :----------------------------------------------------------------------------- | :---------------------------------------------------------------------- | :--------------------------- |
| **Unofficial Skyrim SE Patch (USSEP)**  | Milhares de correções de bugs. **OBRIGATÓRIO.**                                 | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/266)        | Jogo Base + 3 DLCs           |
| **Address Library for SKSE Plugins**    | Permite que mods SKSE funcionem em várias versões do jogo. **OBRIGATÓRIO.**      | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/32444)      | SKSE64                       |
| **SSE Engine Fixes (SKSE64 Plugin)**   | Corrige bugs do motor do Skyrim que o SKSE não cobre. **OBRIGATÓRIO.**           | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/17230)      | SKSE64, Address Lib<br>**Instalação em 2 partes:**<br>1. DLLs manuais na raiz do jogo.<br>2. Mod principal via MO2. (Leia a página do mod!) |
| **SkyUI**                               | Interface moderna para PC (menus, inventário etc). **ESSENCIAL.**                | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/12604)      | SKSE64                       |
| **Static Mesh Improvement Mod (SMIM)**  | Melhora a aparência 3D de milhares de objetos (móveis, cordas...). Base visual. | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/659)        | -                            |
| **PapyrusUtil SE**                      | Biblioteca de scripts usada por muitos mods modernos. Quase obrigatória.         | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/13048)      | SKSE64, Address Lib          |

**Após instalar estes mods, execute o LOOT via MO2 para ordenar os plugins.**

---

## ❓ FAQ e Solução de Problemas Comuns

*   **Crash ao Iniciar (CTD):** Verifique se o SKSE, Address Library e Engine Fixes estão corretamente instalados e são compatíveis com sua versão do jogo. Certifique-se que todos os mods "mestres" (requeridos) estão ativos. Execute o LOOT.
*   **Tela de Carregamento Infinita:** Geralmente conflito de mods ou ordem de carregamento errada. Execute o LOOT. Verifique a página de mods recentes para problemas conhecidos.
*   **Texturas Roxas:** Falta de arquivos de textura. Reinstale o mod que causa o problema (provavelmente SMIM ou outro mod visual se já tiver adicionado mais).
*   **Como Instalar Outros Mods?**
    1.  Baixe via MO2 (botão "Mod Manager Download" no Nexus) ou baixe manualmente e instale pelo ícone 📦 no MO2.
    2.  Ative o mod no painel esquerdo do MO2.
    3.  Verifique se há plugins `.esp`/`.esm` no painel direito (aba Plugins) e se estão ativos.
    4.  **Execute o LOOT** para ordenar.
    5.  Leia a descrição do mod no Nexus para patches de compatibilidade ou instruções especiais!
*   **Onde Pedir Ajuda:** Seção de Posts e Bugs na página do mod no Nexus; [r/skyrimmods](https://www.reddit.com/r/skyrimmods/).

---

**Nota Legal:** Modificar o jogo é por sua conta e risco. Faça backups dos seus saves. Este guia não é afiliado à Bethesda ou Nexus Mods. Use software legítimo.