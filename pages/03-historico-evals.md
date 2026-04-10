# Versionamento e Avaliação (Evals)

Este documento explica como a extensão gerencia o histórico de alterações dos seus prompts.

Após ler este guia, você será capaz de:
* Visualizar as iterações de um prompt.
* Adicionar notas de alteração (Commit messages).
* Avaliar a qualidade de uma versão.
* Restaurar versões anteriores.

---

## Visualizar o histórico de versões

A extensão salva automaticamente o estado anterior de um prompt sempre que você modifica o texto e clica em **Salvar**.

Para visualizar o histórico:
1. Abra um prompt no modo de edição.
2. Clique na aba **Histórico**.
3. A tela exibe uma linha do tempo vertical contendo até as últimas 20 revisões salvas. Cada item lista o número da versão e o horário exato da modificação.

---

## Adicionar notas de alteração

Você pode documentar o motivo de cada alteração para facilitar o rastreamento em projetos longos.

Para adicionar uma nota:
1. Na aba Histórico, localize a versão desejada.
2. Clique no texto de descrição (ex: *"Sem descrição"*).
3. Digite a explicação (ex: *"Aumentei a formalidade do tom"*).
4. Pressione <kbd>Enter</kbd> ou clique no botão de confirmar para salvar.

---

## Avaliar a qualidade (Evals)

Utilize o seletor de 5 estrelas para registrar o desempenho de uma versão específica do prompt.

1. Teste o prompt no AI Studio.
2. Volte à aba Histórico do prompt correspondente.
3. Clique na quantidade de estrelas que representa a qualidade da resposta gerada pelo modelo (1 para ruim, 5 para excelente).

> 💡 **Nota:** Versões marcadas com 5 estrelas recebem um destaque visual amarelo na linha do tempo para identificação rápida.

---

## Restaurar uma versão anterior

Se uma alteração recente prejudicar os resultados do modelo, você pode reverter o texto para uma versão anterior.

Para restaurar um prompt:
1. Na aba Histórico, localize a versão que deseja recuperar.
2. Clique no botão **Restaurar**.
3. Confirme a ação na caixa de diálogo.

A extensão substitui o texto atual no editor pelo texto da versão escolhida. Simultaneamente, a extensão cria um **Backup Automático** (marcado com um ícone azul) do texto que você acabou de substituir, garantindo que nenhum dado seja perdido.