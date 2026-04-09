# 🕒 Histórico & Evals (5 Estrelas)

O **AI Studio Superpowers** trata seus prompts como código. Por isso, incluímos um sistema de versionamento automático que permite experimentar sem medo, sabendo que você pode voltar no tempo a qualquer momento.

---

## 🎞️ A Timeline de Versões

Dentro do Editor de Prompts, a aba **Histórico** exibe uma linha do tempo vertical com todas as iterações do seu prompt.

### Como as versões são criadas?
* **Automático:** Sempre que você edita um prompt e clica em "Salvar", a extensão verifica se houve mudança no texto. Se sim, a versão anterior é movida para o histórico antes de ser substituída.
* **Limite de Segurança:** Para preservar o desempenho e o espaço de armazenamento, mantemos as últimas **20 revisões** de cada prompt.

### Anatomia de um Item na Timeline
Cada registro no histórico contém:
* **Identificador de Versão (v1, v2...):** Numeradas da mais antiga para a mais recente.
* **Carimbo de Data e Hora:** Exatamente quando aquela alteração foi salva.
* **Badges Especiais:** Marcadores que indicam se aquela versão foi um "Backup Automático" (gerado pelo sistema antes de uma restauração).

---

## 📝 Notas de Versão (Commit Messages)

Ao lado de cada versão no histórico, você verá um campo de texto (ou uma mensagem como *"Sem descrição"*). 

Ao clicar nessa mensagem, você pode digitar uma **nota explicativa** sobre o que mudou (ex: *"Ajustei o tom para ser mais formal"* ou *"Removi a restrição de caracteres"*). Isso é fundamental para fluxos de trabalho em equipe ou projetos de longa duração.

---

## ⭐ Sistema de Evals (Avaliação de Qualidade)

Abaixo de cada versão, você encontrará o seletor de **5 Estrelas**. Este não é apenas um adorno visual, mas uma ferramenta de **Benchmarking**:

1. **Teste seu Prompt:** Execute o prompt no AI Studio.
2. **Avalie a Resposta:** Se a resposta do modelo foi perfeita, marque 5 estrelas na versão atual. Se foi ruim, marque apenas 1 ou 2.
3. **Identifique a Melhor Versão:** Versões marcadas com **5 estrelas** ganham um brilho dourado especial na timeline e no ícone de versão, facilitando identificar visualmente qual configuração de prompt gerou o melhor resultado histórico.

---

## ⏪ Restaurando o Passado

Deseja voltar para uma configuração que funcionava melhor?

1. Localize a versão desejada na timeline.
2. Clique no botão **Restaurar**.
3. **Protocolo "Safety First":** A extensão salvará automaticamente o seu rascunho atual como um **Backup de Segurança** e, em seguida, substituirá o editor pelo conteúdo da versão escolhida.

---

## 🛡️ Backups Automáticos

A extensão é vigilante. Se você clicar em "Restaurar" ou realizar uma operação que substitua o conteúdo do editor, o ícone de **Nuvem com Seta** (`settings_backup_restore`) aparecerá no histórico. Isso indica que aquele item foi salvo pelo sistema para garantir que você não perca seu progresso caso mude de ideia após uma restauração.

---

> **Organização Pro:** Você pode usar etiquetas para separar versões de testes. Aprenda a gerenciar sua biblioteca em [Etiquetas (Tags) e Filtros](./06-tags-filtros.md).