# ☁️ Sincronização com GitHub (Nuvem)

Todos os Prompts, Históricos e Anotações criados no **AI Studio Superpowers** são salvos de forma ultrarrápida no banco de dados local do seu navegador. 

Porém, para garantir que você não perca seu trabalho ao trocar de máquina (ou ao limpar o cache do Chrome), nós integramos a extensão diretamente ao **GitHub Gist**.

---

## 🔑 Por que usar o GitHub Gist?
O GitHub Gist é um serviço gratuito da Microsoft/GitHub ideal para guardar pequenos blocos de texto ou arquivos JSON estruturados.
Ao vincular seu Workspace a um Gist, seus dados permanecem **100% privados** e sob o seu controle absoluto. A extensão não possui servidores próprios, nós não temos acesso aos seus prompts.

---

## ⚙️ Passo a Passo: Configuração Inicial

Para ativar a sincronização em um Workspace, você precisa de duas informações do GitHub: um **Token de Acesso** e o **ID de um Gist**.

### 1. Criando o Gist (Banco de Dados)
1. Acesse [gist.github.com](https://gist.github.com/) e faça login.
2. Crie um Gist **Secreto** (Secret Gist) com qualquer nome (ex: `meus_prompts_aistudio.json`). Escreva um `{}` vazio dentro dele apenas para criar o arquivo.
3. Clique em "Create secret gist".
4. Copie o **ID** que aparecer na URL (ex: `https://gist.github.com/SeuUsuario/`**`d43ec0b05b...`**).

### 2. Criando o Token de Acesso (Chave de API)
1. No GitHub, vá em **Settings** > **Developer settings** > **Personal access tokens** > **Tokens (classic)**.
2. Clique em **Generate new token (classic)**.
3. Dê um nome (ex: `AI Studio Sync`) e defina a Expiração (Recomendamos *No expiration* para não precisar refazer isso).
4. Em "Select scopes", marque a caixinha **`gist`** (A extensão precisa apenas desta permissão, nada mais).
5. Clique em Generate e **copie o Token** (ele começa com `ghp_...`).

### 3. Conectando na Extensão
1. No AI Studio, abra a Galeria.
2. Certifique-se de que está no Workspace correto.
3. No rodapé, clique no botão de **Configurações** (Ícone: `settings`).
4. Na aba "GitHub Tradicional", cole o **Gist ID** e o **GitHub Token**.
5. Clique em **Salvar Configuração**. A extensão validará as credenciais imediatamente.

---

## 🔄 Enviando e Recebendo Dados (Push & Pull)

Uma vez configurado, o status no rodapé mudará de *Configurar* para **Ativo** (verde). 

A sincronização **não é automática**. Você tem controle manual para evitar perda acidental de dados:

*   ☁️⬇️ **Sincronizar (Puxar da Nuvem):** Baixa a versão que está salva no GitHub. **Atenção:** Isso substituirá os arquivos locais daquele Workspace. Use essa opção quando acessar de um novo computador.
*   ☁️⬆️ **Enviar (Salvar na Nuvem):** Sobe todos os prompts e notas locais do Workspace atual para o seu GitHub. Faça isso ao fim do seu dia de trabalho para manter um backup seguro.

---

## 🛡️ Status Isolado por Workspace

Lembre-se da [arquitetura de Workspaces](./05-workspaces.md):
Cada Workspace exige sua própria configuração de Nuvem. Você pode usar o mesmo Token para todos, mas é obrigatório que cada Workspace tenha um **Gist ID diferente**, caso contrário, os projetos sobrescreverão os dados uns dos outros no Github.

---

> **Trabalho em Equipe:** Sabia que você pode compartilhar esse Workspace com amigos sem ter que mandar seu Token de acesso privado para eles? Descubra a tecnologia de segurança no [Compartilhamento (Código AISP)](./09-codigo-galeria.md).