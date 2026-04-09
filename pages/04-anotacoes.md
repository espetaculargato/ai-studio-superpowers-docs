# 📌 Anotações e Fragmentos

Nem todo texto salvo é um prompt estruturado. Às vezes, você precisa guardar um bloco de código, uma lista de requisitos, um link de referência ou um rascunho rápido. Para isso, o **AI Studio Superpowers** oferece o módulo de **Anotações**.

---

## 💡 Notas vs. Prompts: Quando usar cada um?

Embora a interface de criação seja similar, o propósito e a integração são diferentes:

*   **Prompts:** São destinados às **Instruções do Sistema**. Eles possuem histórico de versões, evals de estrelas e sobrescrevem o campo de configuração da IA.
*   **Anotações:** São destinadas ao **Corpo da Mensagem (Chat)**. Elas são fragmentos que você "cola" na sua conversa com a IA para fornecer contexto ou exemplos. Também podem ser usados apenas para fazer e salvar anotações.

---

## ⌨️ Injeção Inteligente no Chat

Diferente dos Prompts (que substituem todo o conteúdo), as Notas utilizam um sistema de **Injeção via Cursor**:

1.  Abra a Galeria e vá na aba **Anotações**.
2.  No card da nota desejada, clique no botão **Inserir no Chat**.
3.  **Onde o texto vai parar?** A extensão identifica a posição exata do seu cursor (caret) dentro da caixa de chat do Google AI Studio e insere a nota naquele ponto específico. 

---

## 🎨 Organização Visual

As anotações são visualmente distintas na Galeria para evitar confusão:
*   Utilizam o ícone de **Nota Adesiva** (`sticky_note_2`).
*   A cor de destaque padrão é sutil para não cansar a vista durante leituras longas.
*   Assim como os prompts, as notas suportam o sistema de **Etiquetas (Tags)**, permitindo filtrar, por exemplo, apenas notas de "Documentação" ou "Snippets de Código".

---

## 📝 Editor de Notas

O editor de notas é otimizado para escrita fluida:
*   **Título Opcional:** Se você não der um título, a extensão salvará automaticamente como *"Sem Título"*.
*   **Monaco Editor:** O suporte a Markdown e realce de sintaxe de código também está presente aqui, tornando as notas o lugar perfeito para guardar bibliotecas de funções que você costuma enviar para a IA analisar.

---

> **Dica Pro:** Mantenha suas anotações organizadas por projetos usando os **Workspaces**. Saiba como separar seus contextos em [Workspaces (Isolamento)](./05-workspaces.md).