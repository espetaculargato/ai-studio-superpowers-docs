# Sincronizar com o GitHub

Este documento explica como vincular seu Workspace a um repositório na nuvem para realizar backups e acessos remotos.

Após ler este guia, você será capaz de:
* Criar credenciais no GitHub.
* Configurar o armazenamento na extensão.
* Executar sincronizações manuais (Push e Pull).

A extensão utiliza o **GitHub Gist** como infraestrutura de nuvem. Seus dados permanecem privados no seu repositório, sem passar por servidores de terceiros.

---

## Obter credenciais do GitHub

Você precisa de um Gist (para armazenar o arquivo) e de um Token (para autorizar a escrita).

**Passo A: Criar o Gist**
1. Acesse [gist.github.com](https://gist.github.com/).
2. Escreva `{}` no campo de conteúdo.
3. Clique em **Create secret gist**.
4. Copie o ID contido no final da URL gerada.

**Passo B: Gerar o Token de Acesso**
1. No GitHub, acesse **Settings > Developer settings > Personal access tokens > Tokens (classic)**.
2. Clique em **Generate new token (classic)**.
3. Na seção "Select scopes", marque a opção `gist`.
4. Clique em **Generate token** e copie a chave resultante (inicia com `ghp_`).

---

## Configurar a extensão

Cada Workspace exige sua própria configuração de nuvem. Recomenda-se utilizar o mesmo Token, mas um Gist ID distinto para cada Workspace.

Para vincular o Workspace atual:
1. Abra a Galeria e clique no botão de **Configurações**.
2. Cole o **Gist ID** e o **GitHub Token** nos respectivos campos.
3. Clique em **Salvar Configuração**. A extensão validará as credenciais.

---

## Executar sincronização (Push & Pull)

A sincronização de dados ocorre exclusivamente de forma manual. 

Para sincronizar, utilize os botões com ícones de nuvem localizados no rodapé da Galeria:

*   **Sincronizar (Seta para baixo):** Baixa o arquivo do GitHub e substitui os dados do Workspace local atual. Utilize ao acessar a extensão a partir de um novo computador.
*   **Enviar (Seta para cima):** Salva os dados do Workspace local atual no GitHub, sobrescrevendo a versão da nuvem. Utilize para gerar backups após uma sessão de trabalho.