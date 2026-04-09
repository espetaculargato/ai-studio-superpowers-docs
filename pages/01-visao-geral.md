# 🚀 Visão Geral & Interface

Bem-vindo ao **AI Studio Superpowers**. Esta extensão foi projetada para transformar o Google AI Studio em uma verdadeira IDE (Ambiente de Desenvolvimento Integrado) para Engenharia de Prompts. 

Nossa arquitetura foi construída para se camuflar perfeitamente à interface nativa do Google, respeitando os temas Claro e Escuro automaticamente, sem causar lentidão ou consumir memória excessiva.

---

## 📍 Onde encontrar as ferramentas?

Após instalar a extensão, você não precisa abrir popups externos complexos. A extensão injeta seus controles de forma cirúrgica diretamente na interface do AI Studio:

1. **Botão de Galeria (Hub Principal):** 
   Localizado logo abaixo do painel de **Instruções do Sistema** (System Instructions). Clicar neste botão abrirá o seu banco de dados central de Prompts e Notas.
   
   *![Localização do Botão Galeria](../images/print-botao-galeria.png)* <!-- Dica: Salve um print com este nome na pasta images/ do seu Github -->

2. **Botão de Exportação de Chat:** 
   Localizado no canto superior direito do painel de Chat, ao lado dos botões nativos de configurações de execução do modelo.

---

## 🖼️ O Hub Principal (A Galeria)

Ao clicar no botão "Galeria", você entra na interface principal da extensão. Este painel flutuante (Modal) foi desenhado para ser sua "Sala de Controle".

### Elementos da Interface
* **Barra Superior (Toolbar):** Contém a barra de pesquisa em tempo real e os atalhos rápidos das suas Etiquetas (Tags).
* **Navegação (Abas):** Alterne rapidamente entre seus **Prompts** (textos estruturados) e **Anotações** (fragmentos e rascunhos).
* **Botões Flutuantes (FAB):** No canto inferior direito, você encontrará os botões para **Criar Novo** (`+`) ou **Importar** o texto que já está digitado atualmente no AI Studio.
* **Rodapé de Sistema:** Onde você gerencia seus [Workspaces](./05-workspaces.md) (Projetos isolados) e a [Sincronização com a Nuvem](./08-sincronizacao.md).

---

## 🎛️ Controle de Layout e Ordenação

Seu banco de dados se adapta à sua necessidade de foco. No canto superior direito da tela principal, você encontrará o seletor de **Layouts**:

* 🔲 **Galeria:** Modo padrão (Cards grandes). Ideal para visualizar títulos e descrições longas. Suporta coloração dinâmica caso você use Emojis nos títulos.
* ⏹️ **Compacto:** Reduz o preenchimento (padding) dos cards, permitindo visualizar mais prompts na mesma tela.
* 📄 **Lista:** Oculta as descrições e transforma a interface em uma tabela super enxuta. Excelente para Workspaces com dezenas de prompts.

### Arrastar e Soltar (Drag & Drop)
A ordem dos seus prompts e anotações é totalmente personalizável. Basta **clicar, segurar e arrastar** qualquer card para reorganizar sua área de trabalho. Uma linha guia azul (indicador visual) mostrará exatamente onde o item será solto. 

A nova ordem é salva automaticamente no seu HD instantaneamente.

---

> **Próximo Passo:** Aprenda a criar, editar e injetar seu primeiro prompt lendo a sessão [Criando e Injetando Prompts](./02-gerenciamento-prompts.md).