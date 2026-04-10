# 🤝 Compartilhamento (Código AISP)

Trabalhar em equipe exige que todos tenham acesso à mesma biblioteca de prompts. O método tradicional (enviar o Gist ID e seu Token Privado do GitHub pelo Slack ou WhatsApp) é demorado e expõe sua chave de forma explícita.

Para resolver isso, o **AI Studio Superpowers** possui um gerador de **Códigos de Galeria (AISP)** integrado.

---

## 🔐 O que é um Código AISP?

É uma string (texto) que encapsula o seu Gist ID e o Token do GitHub usando uma criptografia simples (Cifra XOR + Base64). 

Embora **não seja de nível militar**, ele cumpre um papel fundamental de **ofuscação**: impede que leitores automáticos (scrapers) ou olhos curiosos leiam sua chave imediatamente ao olhar para o chat da empresa.

*Exemplo de um Código AISP gerado:*
`AISP::Tz1zMjB3eD46RDA3NDg1bHAwYzY...`

---

## 📤 Como Gerar e Compartilhar

Se você já configurou as suas credenciais no Workspace e quer enviar o acesso para um colega:

1. Na Galeria da sua extensão, clique em **Configurações** no rodapé.
2. Certifique-se de que os campos Gist ID e Token estão preenchidos na aba "GitHub Tradicional".
3. Clique no botão inferior **"Criar código de Galeria"** (Ícone: `content_copy`).
4. O botão mudará rapidamente para "Check" (Verde), indicando que o código mascarado foi copiado para sua área de transferência.
5. Cole esse código no Slack, Discord ou E-mail e envie para a sua equipe.

> ⚠️ **Nota de Segurança:** Qualquer pessoa com a extensão instalada e com esse código poderá ler e sobrescrever os dados no Gist vinculado. Compartilhe **apenas com pessoas de confiança**.

---

## 📥 Como Importar (Vincular-se a uma Equipe)

Se alguém te enviou um código `AISP::`, seguir estas etapas conectará o seu computador ao Workspace compartilhado em segundos:

1. Abra a Galeria e crie um **Novo Workspace** (ex: "Prompts do Projeto X").
2. No rodapé, clique no ícone de **Configurações**.
3. Na parte superior do modal de configurações, troque para a aba **Código de Galeria**.
4. Cole o código completo (incluindo o prefixo `AISP::`) na caixa de texto.
5. Clique em **Salvar Configuração**.

A extensão irá decodificar as credenciais, realizar uma validação de segurança com a API do GitHub e, se estiver tudo correto, conectará seu Workspace.

**Último Passo:** Após conectar com sucesso, não esqueça de voltar à tela inicial da Galeria e clicar no botão **Sincronizar (Nuvem para o PC)** no rodapé para baixar os prompts da equipe para a sua máquina!

---

## 🔄 Finalizando a Jornada

Com isso, você tem o poder completo da Engenharia de Prompts e de Colaboração diretamente dentro da interface oficial do Google.

Explore, faça iterações, marque 5 estrelas nas suas melhores versões e eleve seu fluxo de trabalho de IA para o próximo nível. 

**Bem-vindo ao AI Studio Superpowers!** 🚀