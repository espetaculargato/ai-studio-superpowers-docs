# 🏢 Workspaces (Isolamento de Projetos)

Quando você passa a usar o Google AI Studio profissionalmente, sua biblioteca de prompts cresce rapidamente. Para evitar desordem e limites técnicos, o **AI Studio Superpowers** possui um sistema completo de **Workspaces**.

Um Workspace é como um "HD virtual isolado". Prompts, Anotações, Etiquetas e até Credenciais de Nuvem de um Workspace não se misturam com os de outro.

---

## 🗄️ O Menu de Workspaces

Você encontrará o gerenciador de Workspaces na **barra de rodapé** do painel da Galeria (lado direito). O botão exibe o nome do seu projeto ativo atual.

### Ações Disponíveis no Menu:
Ao clicar no nome do Workspace, um menu suspenso (Dropdown) se abre. Nele, você pode:
*   **Trocar de Ambiente:** Clique sobre qualquer nome para carregar os dados daquele projeto. A transição é quase instantânea e limpa a tela de trabalho anterior.
*   **Novo Workspace:** Use o botão `+ Novo Workspace` no final da lista para criar ambientes para clientes, equipes ou estudos específicos.
*   **Renomear (`edit`):** Permite alterar o nome do projeto ativo ou inativo.
*   **Excluir (`delete`):** Remove o workspace e **apaga permanentemente** todos os prompts e notas associados a ele. (Sempre exibimos um aviso de confirmação antes de apagar).

---

## 🔄 Reordenando a Lista (Drag & Drop)

Sua lista de Workspaces está crescendo? Você pode reordenar o menu para manter seus projetos mais importantes no topo.
1.  Abra o menu de Workspaces.
2.  Clique e segure qualquer item da lista.
3.  Arraste-o para cima ou para baixo. Uma linha azul indicará a nova posição.
4.  Solte o mouse. A nova ordem é salva imediatamente no seu navegador.

---

## 🔒 Segurança e Credenciais Isoladas

A maior vantagem da arquitetura de Workspaces é o isolamento de dados na nuvem.
*   As configurações do GitHub Gist (Token e ID) são atreladas **exclusivamente** ao Workspace atual.
*   Isso significa que você pode sincronizar seu "Workspace Pessoal" com o seu GitHub privado, e sincronizar o "Workspace da Empresa" com o GitHub corporativo, sem que um sobrescreva o outro.
*   Para saber mais sobre como configurar a nuvem, visite a sessão de [Sincronização com GitHub](./08-sincronizacao.md).

---

## 💾 Prevenção de "Quota Exceeded"

*Curiosidade Técnica:* O Google Chrome impõe um limite estrito de armazenamento (cerca de 5MB) por chave de dados locais em extensões. 
Se tentássemos salvar todos os seus prompts do mundo em um único arquivo, a extensão falharia. O sistema de Workspaces resolve isso "fragmentando" o banco de dados. Cada Workspace é um arquivo separado no seu disco rígido, permitindo que você tenha um volume praticamente infinito de prompts sem nunca estourar a memória do navegador.

---

> **Mantenha a Ordem:** Dentro do seu Workspace, a organização continua através das Tags. Descubra como gerenciá-las em [Etiquetas (Tags) e Filtros](./06-tags-filtros.md).