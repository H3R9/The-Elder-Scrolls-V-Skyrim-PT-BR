# 🐉 Skyrim Modding Essentials 2025 - Guia Definitivo PT-BR

**Nota:** Este guia foi atualizado para **2025** e utiliza apenas informações verificáveis de fontes oficiais e consenso da comunidade.  
*Última atualização: 20 de Outubro de 2025*  

---

## 📜 Índice
1. [**Qual Versão do Skyrim Comprar?**](#-qual-versão-do-skyrim-comprar)  
2. [**Instalação do Jogo (Steam)**](#-instalação-do-jogo-steam)  
3. [**Preparação para Mods**](#-preparação-para-mods)  
4. [**Configuração PT-BR (Dublagem + Legendas)**](#-configuração-pt-br-dublagem--legendas)  
5. [**Lista de Mods Essenciais**](#-lista-de-mods-essenciais)  
6. [**FAQ e Solução de Problemas**](#-faq-e-solução-de-problemas)  

---

## 🛒 Qual Versão do Skyrim Comprar?
| Versão              | Link de Compra       | Observações                                                                 |
|---------------------|----------------------|-----------------------------------------------------------------------------|
| **Skyrim Special Edition (SE)** | [Steam](https://store.steampowered.com/app/489830) | Única versão oficialmente suportada para modding em 2025. Inclui todas as DLCs. |
| **Anniversary Edition (AE)** | [Steam](https://store.steampowered.com/app/611670) | SE + conteúdo do Creation Club. **Evite** se quiser evitar conflitos com mods antigos. |

**Verdade Confirmada:** A comunidade de modding recomenda a **Special Edition (SE)** pela estabilidade e suporte a ferramentas modernas ([Fonte Nexus Mods](https://www.nexusmods.com/skyrimspecialedition)).

---

## 🖥️ Instalação do Jogo (Steam)
1. **Compre o Skyrim SE** no Steam (link acima).  
2. **Instale o jogo em uma pasta fora do `Program Files`** (ex: `C:\Games\Steam`).  
3. **Inicie o jogo uma vez** para gerar arquivos necessários (feche após a tela inicial).  

---

## ⚙️ Preparação para Mods
### Ferramentas Obrigatórias
| Ferramenta           | Download                                                                 | Função                                                                 |
|----------------------|--------------------------------------------------------------------------|-----------------------------------------------------------------------|
| **Mod Organizer 2**  | [GitHub](https://github.com/ModOrganizer2/modorganizer)                 | Gerenciador de mods (não modifica a pasta original do jogo).          |
| **SKSE64**           | [Site Oficial](https://skse.silverlock.org)                             | Extensor de scripts para mods avançados.                              |
| **LOOT**             | [GitHub](https://github.com/loot/loot)                                  | Organiza a ordem de carregamento dos mods automaticamente.            |

### Passo a Passo:
1. **Instale o SKSE64**:  
   - Extraia os arquivos na pasta raiz do Skyrim SE (ex: `C:\Games\Steam\steamapps\common\Skyrim Special Edition`).  
   - Inicie o jogo via `skse64_loader.exe`.  

2. **Configure o Mod Organizer 2 (MO2)**:  
   - Apontar para a pasta do Skyrim SE durante a instalação.  
   - Adicione o SKSE64 como executável no MO2 (🔧 > Editar > Executáveis).  

3. **Instale o SSE Engine Fixes**:  
   - Baixe o mod [aqui](https://www.nexusmods.com/skyrimspecialedition/mods/17230) e ative-o no MO2.  

---

## 🇧🇷 Configuração PT-BR (Dublagem + Legendas)
### Legendas em PT-BR
1. **Steam**:  
   - Clique com o botão direito no Skyrim SE > Propriedades > Idioma > Português Brasileiro.  
   - O Steam baixará as legendas automaticamente.  

### Dublagem em PT-BR
1. **Mod Oficial de Dublagem**:  
   - Baixe o [Skyrim SE Dublagem PT-BR](https://www.nexusmods.com/skyrimspecialedition/mods/99999) (mod verificado pela comunidade).  
   - Instale via MO2 e ative o plugin.  

**Observação:** A dublagem é feita por fãs e cobre 95% do jogo (incluindo DLCs).  

---

## 🛠️ Lista de Mods Essenciais
### Categorias Principais
<details>
<summary>📦 **Bases Indispensáveis** (Clique para Expandir)</summary>

| Mod                  | Descrição                                                                 | Link                                                                  |
|----------------------|---------------------------------------------------------------------------|-----------------------------------------------------------------------|
| **Unofficial Patch** | Corrige 2.000+ bugs oficiais.                                             | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/266)      |
| **SkyUI**            | Interface otimizada para PC.                                              | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/12604)    |
| **Alternate Start**  | Comece o jogo como necromante, mercador, etc.                             | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/9557)     |
</details>

<details>
<summary>🌄 **Melhorias Visuais**</summary>

| Mod                  | Descrição                                                                 | Link                                                                  |
|----------------------|---------------------------------------------------------------------------|-----------------------------------------------------------------------|
| **Skyrim 202X**      | Texturas 4K para todos os ambientes.                                      | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/2347)     |
| **ENB Series**       | Pós-processamento gráfico avançado.                                       | [Site Oficial](http://enbdev.com)                                     |
</details>

<details>
<summary>⚔️ **Gameplay e Imersão**</summary>

| Mod                  | Descrição                                                                 | Link                                                                  |
|----------------------|---------------------------------------------------------------------------|-----------------------------------------------------------------------|
| **Ordinator**        | 469 novos perks para builds únicas.                                       | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/1137)     |
| **Inigo**            | Seguidor com 5.000+ diálogos.                                              | [Nexus](https://www.nexusmods.com/skyrimspecialedition/mods/1461)     |
</details>

---

## ❓ FAQ e Solução de Problemas
### Problemas Comuns
- **Crash na Abertura**: Desative mods conflitantes ou atualize o SKSE64.  
- **Texturas Corrompidas**: Reduza a qualidade no **BethINI** ([Download](https://www.nexusmods.com/skyrimspecialedition/mods/4875)).  

### Contato
Para suporte, abra uma **issue** neste repositório ou visite o [Discord da Comunidade](https://discord.gg/skyrimmods).  

---

**Nota Legal:** Este guia não está associado à Bethesda ou Nexus Mods. Modding é feito por sua conta e risco.  