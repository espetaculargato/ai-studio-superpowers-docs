# 🏗️ Criando e Injetando Prompts

O gerenciamento de prompts é a funcionalidade central do **AI Studio Superpowers**. Nossa interface substitui campos de texto simples por um ambiente de edição de nível profissional, integrado ao fluxo de trabalho nativo.

---

## 🛠️ O Painel de Edição

Ao criar um novo prompt ou editar um existente, você terá acesso a três áreas fundamentais:

1. **Cabeçalho de Identificação:** Onde você define o título do seu prompt. 
   * **Dica Visual:** Se você iniciar o título com um **Emoji** (ex: `🐍 Script Python`), a extensão detectará a cor dominante do emoji e colorirá o card na galeria automaticamente para facilitar a identificação visual.

2. **Sistema Inline de Etiquetas (Tags):** 
   Localizado logo abaixo do título, este campo permite categorizar seus prompts. 
   * Ao digitar uma nova tag, a extensão sugere etiquetas já existentes no seu banco de dados para evitar duplicatas.
   * Pressione `Enter` ou `,` para confirmar uma tag.

3. **Área de Conteúdo (Monaco Editor):**
   Utilizamos o **Monaco Editor** (o motor que alimenta o VS Code). Isso garante:
   * **Syntax Highlighting:** Coloração de código para Markdown e linguagens de programação.
   * **Numeração de Linhas:** Essencial para prompts extensos e complexos.

---

## 🚀 O Poder da Injeção Direta

A principal vantagem desta extensão é a capacidade de "teleportar" seu prompt salvo diretamente para os campos do Google AI Studio com um único clique.

### Inserir nas Instruções do Sistema
Dentro do editor ou no menu de contexto do card, você encontrará o botão **"Inserir nas Instruções"**. 
* **Fluxo de Segurança:** Se o campo de Instruções do Sistema no Google já estiver preenchido, a extensão exibirá um diálogo de confirmação para evitar que você apague seu trabalho atual por acidente.

### Inserir no Chat
Para fragmentos de prompts ou exemplos de poucas linhas, você pode usar a opção de inserir (Menu de Contexto) diretamente na caixa de mensagem ativa . O texto será inserido exatamente na posição onde o seu cursor (caret) estiver piscando.

---

## 🖱️ Ações Rápidas (Menu de Contexto)

Você pode realizar operações avançadas sem sequer abrir o editor de prompts. Clique com o **botão direito do mouse** sobre qualquer card na galeria para acessar:

* **Duplicar:** Cria um clone exato do prompt selecionado (incluindo tags e conteúdo), mas reseta o histórico de versões. Útil para criar variações de um mesmo "Prompt Base".
* **Copiar Conteúdo:** Copia o texto bruto para sua área de transferência (Clipboard).
* **Excluir:** Remove permanentemente o item do Workspace atual.

---

## 📥 Importando do AI Studio

Se você acabou de escrever um prompt excelente diretamente na interface do Google e deseja salvá-lo na sua galeria:
1. Abra a Galeria.
2. No canto inferior direito, ao lado do botão de (+), clique no botão **Importar do Chat**.
3. A extensão capturará automaticamente o texto que está nas "Instruções do Sistema" e abrirá o editor com o conteúdo já preenchido para você dar um título e salvar.

---

> **Acompanhamento de Mudanças:** Toda vez que você edita e salva um prompt, a extensão cria uma "foto" do estado anterior. Saiba mais em [Histórico & Evals](./03-historico-evals.md).