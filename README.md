# HUNTERA Companion

Navegador para Windows feito para o [HUNTERA](https://huntera.com.br): até **4 contas** numa janela só, um **modo leve** para PC fraco e um painel com os dados das suas hunts e do seu patrimônio.

Projeto independente, sem vínculo com o HUNTERA.

## ⬇️ Baixar
Vá em **[Releases](../../releases/latest)** e baixe `HUNTERA-Companion-Setup-<versão>.exe`.

- Windows 10 ou 11 (64 bits). Não precisa de administrador nem de Node.js.
- Na primeira vez o Windows pode mostrar **"O Windows protegeu o computador"**, porque o instalador não tem assinatura digital paga. Clique em **Mais informações → Executar assim mesmo**.
- Confira o arquivo pelo SHA-256 publicado em cada Release.

## O que ele faz
- **4 contas isoladas:** cada conta tem o próprio login e os próprios dados, então entrar numa não derruba a outra.
- **Mosaico, Abas e Analyzer:**
  - Mosaico mostra as contas lado a lado;
  - Abas mostra uma por vez;
  - Analyzer mostra só os dados, com o jogo de todas as contas parado de desenhar e elas continuando a caçar.
- **Economia e Ultra Light:** a conta que não está na tela para de desenhar o jogo e sai da memória RAM. Com 4 contas no jogo, o app fica em torno de **500 MB** no Gerenciador de Tarefas.
- **Analyzer:**
  - **Party ao vivo:** XP/h, balance/h, DPS, vida, mana, stamina, drops e a hunt atual de cada personagem.
  - **Análises:** XP e balance por dia, médias, comparação com o período anterior e filtros por conta, personagem e party.
  - **Patrimônio:** gold na mochila, no baú e em ordens de compra, além das coins. Transferências entre os seus personagens não contam como lucro.
  - **Leilão de Huntera Coin:** preço, spread, tendência e o histórico das suas negociações.
  - **Vendas por dinheiro:** registre o valor das suas vendas e veja os compradores agrupados.
  - **Valores em gold, R$ ou US$**, pela cotação atual.
- **Avisos do Windows** (desligados por padrão): conta saiu do jogo, personagem morreu, personagem parado na hunt, stamina baixa.
- **Backup do histórico** pelo próprio app.

## O que ele NÃO faz
- **Não joga por você:** nada de bot, macro, movimentação, combate, coleta, uso de item ou login automático. Você clica em **Jogar** em cada conta.
- **Não mexe no jogo:** não injeta scripts e não envia nada ao servidor. Os dados vêm só da leitura da conexão do próprio cliente oficial, a mesma que a aba Network do navegador mostra.
- **Não usa conexão própria com o servidor:** o jogo roda sempre na página oficial.
- **Não guarda senha** e não copia os seus cookies. O login é feito por você, no site oficial.
- **Respeita o limite oficial de 4 contas.**

## Privacidade
- Tudo fica só no seu PC, em `%APPDATA%\HUNTERA Companion\`. Nada é enviado para fora.
- Nomes de outros jogadores não são gravados. A única exceção é o comprador de uma venda que **você** confirmou.
- Chat e mensagens privadas não são lidos.

## Atualizar
Feche o app e rode o instalador da versão nova por cima da antiga. Seus dados e logins continuam.

## Backup e restauração
- **Fazer backup:** use **Dados → Fazer backup do histórico…**. Os logins não entram no backup.
- **Restaurar:**
  1. Feche o app.
  2. Copie o arquivo do backup para `%APPDATA%\HUNTERA Companion\data\companion.db`.
  3. Apague `companion.db-wal` e `companion.db-shm`, se existirem.
  4. Abra o app.

## Desinstalar
Use **Configurações → Aplicativos → HUNTERA Companion → Desinstalar**. Para apagar também o histórico e os logins, apague a pasta `%APPDATA%\HUNTERA Companion\`.
