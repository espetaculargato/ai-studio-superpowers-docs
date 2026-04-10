# Compartilhar Configurações (AISP)

Este documento descreve como gerar e importar códigos ofuscados para compartilhar o acesso à nuvem com sua equipe.

Após ler este guia, você será capaz de:
* Entender a função do código AISP.
* Gerar um código a partir de credenciais existentes.
* Importar um código para conectar-se a uma equipe.

---

## O que é um Código AISP

O código de Galeria (AISP) é uma string de texto que condensa o Gist ID e o Token do GitHub. 
A extensão aplica uma ofuscação (Base64) neste código para evitar que rastreadores automáticos capturem suas credenciais quando o texto é enviado via aplicativos de mensagens corporativas.

> ⚠️ **Atenção:** Esta ofuscação não é uma criptografia avançada. Compartilhe os códigos apenas com membros confiáveis da sua equipe. Quem possuir o código poderá modificar os arquivos do repositório no GitHub.

---

## Gerar um código de compartilhamento

Para exportar o acesso do seu Workspace atual:

1. Certifique-se de que a configuração na aba "GitHub Tradicional" foi concluída e salva.
2. Clique no botão de **Configurações** no rodapé da Galeria.
3. Clique no botão **Criar código de Galeria**. O botão mudará de cor indicando que o código foi copiado para a área de transferência.
4. Cole e envie o código `AISP::...` para os membros da sua equipe.

---

## Importar um código de equipe

Se você recebeu um código da sua equipe, você precisa conectá-lo a um Workspace limpo.

Para importar um código:
1. Na Galeria, clique no menu de rodapé e selecione **+ Novo Workspace**.
2. Abra as **Configurações**.
3. Selecione a aba **Código de Galeria** (na parte superior do painel).
4. Cole o texto completo na caixa de texto.
5. Clique em **Salvar Configuração**.
6. Após a conexão bem-sucedida, feche as configurações e clique no botão **Sincronizar (Seta para baixo)** no rodapé para baixar os dados da equipe para sua máquina local.