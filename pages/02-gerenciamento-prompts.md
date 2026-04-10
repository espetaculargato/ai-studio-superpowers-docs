# Gerenciar Prompts

Este documento descreve como criar, editar e inserir prompts no Google AI Studio. 

Após ler este guia, você será capaz de:
* Criar e formatar um prompt no Monaco Editor.
* Inserir prompts nas Instruções do Sistema ou no Chat.
* Executar ações rápidas através do menu de contexto.
* Importar textos da interface para a extensão.

---

## Editar um prompt

A tela de edição substitui os campos de texto padrão por um ambiente estruturado. Para editar um prompt:

1. Clique no botão **Criar Novo** (`+`) na Galeria, ou clique no ícone de edição em um card existente.
2. Defina o **Título**. Se você iniciar o título com um emoji, a extensão usará a cor desse emoji para destacar o card na Galeria.
3. Adicione **Etiquetas (Tags)** para categorizar o prompt.
4. Escreva o texto na **Área de Conteúdo**. Esta área utiliza o Monaco Editor, que fornece numeração de linhas e realce de sintaxe (Syntax Highlighting) para Markdown e linguagens de programação.

---

## Inserir prompts no AI Studio

Você pode transferir o conteúdo salvo na extensão diretamente para os campos do Google AI Studio.

### Substituir as Instruções do Sistema
Para preencher o painel principal de comportamento do modelo:
1. Localize o prompt desejado na Galeria.
2. Clique com o botão direito sobre o card e selecione **Inserir nas Instruções**. (Na aba prompts essa ação pode ser feita apenas clicando no card).
3. Se o campo nativo do Google já possuir texto, confirme a substituição na caixa de diálogo. A extensão injetará o texto e atualizará o estado da página automaticamente.

### Inserir na mensagem (Chat)
Para adicionar fragmentos menores à conversa ativa:
1. Localize o prompt na Galeria.
2. Clique com o botão direito sobre o card e selecione **Inserir na Mensagem**. 
A extensão insere o texto exatamente na posição atual do seu cursor.

---

## Executar ações rápidas

Utilize o menu de contexto para gerenciar seus cards sem abrir a tela de edição. Clique com o **botão direito** sobre qualquer card para acessar as seguintes opções:

*   **Editar:** Abre o painel completo de modificação.
*   **Duplicar:** Cria uma cópia exata do prompt e de suas etiquetas, mas descarta o histórico de versões.
*   **Copiar Conteúdo:** Copia o texto bruto para a área de transferência.
*   **Excluir:** Remove o item do Workspace de forma permanente.

---

## Importar texto do AI Studio

Para salvar um texto que você acabou de digitar na interface nativa do Google:
1. Abra a Galeria.
2. Clique no botão **Importar do Chat** (ícone de atalho), localizado no canto inferior direito.
3. A extensão captura o texto atual das Instruções do Sistema e abre o editor para que você defina um título e o salve.