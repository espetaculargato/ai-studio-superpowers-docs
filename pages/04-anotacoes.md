# Gerenciar Anotações

Este documento descreve como utilizar o módulo de Anotações para armazenar fragmentos de texto e contexto auxiliar.

Após ler este guia, você será capaz de:
* Distinguir Anotações de Prompts.
* Inserir anotações no fluxo do chat.
* Organizar e criar notas.

---

## Comparar Prompts e Anotações

Embora compartilhem a mesma interface de criação, Prompts e Anotações possuem propósitos distintos:

| Característica | Prompts | Anotações |
| :--- | :--- | :--- |
| **Objetivo** | Configurar o comportamento principal da IA. | Armazenar contexto, links, código ou rascunhos. |
| **Destino de Injeção** | Painel de *System Instructions*. | Caixa de entrada de mensagens do *Chat*. |
| **Versionamento** | Mantém histórico de 20 versões e suporte a *Evals*. | Não possui histórico de versões. |

---

## Inserir anotações na mensagem

As anotações utilizam injeção baseada em cursor, permitindo concatenar múltiplos fragmentos em uma única mensagem.

Para injetar uma nota:
1. Clique na caixa de chat do AI Studio e posicione o cursor de texto no local exato onde deseja inserir o fragmento.
2. Abra a Galeria e selecione a aba **Anotações**.
3. Clique no botão **Inserir na Mensagem** no card da anotação desejada.

---

## Criar e importar anotações

O editor de anotações possui os mesmos recursos de formatação (Monaco Editor) presentes nos prompts. O título é opcional; se você deixar em branco, a extensão salvará o item como *"Sem Título"*.

Para extrair um texto da tela e transformá-lo em nota:
1. Acesse a aba **Anotações** na Galeria.
2. Clique no botão **Importar do Chat**.
3. A extensão prioriza a captura do texto atualmente digitado na caixa de entrada do usuário. O editor abrirá com o conteúdo pronto para salvamento.