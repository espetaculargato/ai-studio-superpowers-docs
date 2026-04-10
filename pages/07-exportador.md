# Exportar Conversas

Este documento explica como utilizar o Exportador para salvar o histórico de chat em um arquivo limpo e formatado.

Após ler este guia, você será capaz de:
* Acionar a exportação e escolher o formato de saída.
* Entender o requisito de recarregamento da página.
* Incluir ou remover blocos de "Pensamento" da IA.

---

## Acionar a exportação

A extensão intercepta o tráfego de rede da API do Google para gerar documentos Markdown íntegros.

Para exportar o chat atual:
1. Clique no ícone de **Exportação** localizado no canto superior direito da tela do AI Studio (ou no ícone da extensão no Chrome).
2. Selecione a ação desejada:
   * **Copiar Sessão:** Envia o texto para a sua área de transferência.
   * **Baixar Sessão:** Salva o arquivo localmente com a extensão `.txt`.

---

## Entender o requisito de recarregamento

Ao iniciar a exportação, a extensão solicitará permissão para recarregar a página.

*   **O Problema:** A interface nativa do Google remove elementos antigos da tela para economizar memória (DOM virtualization). Extrair o texto visível resultaria em dados incompletos.
*   **A Solução:** Ao aceitar o recarregamento, a extensão intercepta o pacote de dados (JSON) direto do servidor do Google durante o processo de carregamento. Isso garante a extração completa do histórico, sem vazamento de tags HTML. A cópia ou o download ocorre silenciosamente após a conclusão do recarregamento.

---

## Configurar blocos de pensamento

Se você utiliza modelos focados em raciocínio (série *Thinking*), pode decidir se deseja manter os fluxos de pensamento no arquivo final.

Para alterar esta configuração:
1. Clique no ícone de **Exportação** no AI Studio.
2. Alterne a chave **Incluir Pensamentos**.
   * Quando ativado, a extensão cria seções `### [Thought Process]` contendo as deliberações do modelo antes da resposta final.
   * Quando desativado, apenas a resposta final do modelo é exportada.