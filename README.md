# ShadowLurk - Sua Ferramenta Definitiva para Twitch

ShadowLurk é uma extensão de navegador desenvolvida por [**Felipenor**.](https://linkbio.co/felipenor) para automatizar o lurk (assistir streams em segundo plano), coletar pontos de canal e baixar emotes com facilidade.

## ✨ Atualizações Recentes

- Versão atual: `v2.5`.
- A verificação de lives agora pode usar a conexão oficial da Twitch com um botão só no popup, sem pedir Client ID nem Redirect URI para o usuário.
- As opções de recarga automática das lives e conexão oficial com a Twitch agora ficam dentro do menu de configurações acessado pelo ícone de engrenagem no canto superior esquerdo.
- A conexão oficial com a Twitch foi ajustada e agora conclui a autorização corretamente pelo popup.
- O áudio das lives agora respeita o desmute manual do usuário e não volta a mutar sozinho depois de alguns instantes.
- O aviso de raid foi reforçado para aparecer de forma mais confiável, inclusive quando o Twitch muda de rota.
- A navegação de raid foi refinada para manter a live raidada aberta até o usuário fechar e fechar a origem automaticamente quando ela realmente ficar offline.
- O popup ganhou uma nova opção opcional para fechar guias quando a live terminar, com modo para fechar todas, só canais escolhidos ou manter desativado. Se o modo selecionado ficar sem nenhum canal marcado, as lives continuam abertas.
- A lista de canais fixos foi atualizada e agora inclui `baluartetm`, `kiolhawuz`, `alphaieslis`, `rafael_1225`, `b3lialtv`, `rarutosusto` e outros parceiros da ShadowLurk.
- A popup ganhou uma blacklist para bloquear canais que a extensão não deve abrir automaticamente.
- O botão de desligar agora separa melhor as duas ações: só desligar a extensão ou desligar e fechar todas as lives abertas, sem derrubar o VOD do Felipenor no desligar simples.
- A extensão ganhou uma opção opcional de recarga automática das lives abertas, com intervalo configurável pelo usuário, timer visível no popup e recarga real das guias no horário certo, sem recarregar antes do tempo configurado.
- O popup agora permite exportar e importar os canais favoritos em arquivo para facilitar atualizações da extensão sem precisar digitar tudo de novo.
- O arquivo de backup também pode levar a blacklist, para você não perder seus bloqueios personalizados.
- O popup de raid recebeu um fallback para aparecer também em mudanças de rota do Twitch.
- A interface ganhou seletor de idioma no popup e também na página do formulário de inscrição.
- O botão do Linkbio foi atualizado para `https://linkbio.co/Felipenor`.
- A inscrição para virar fixo agora é enviada via Formspree.

## 🚀 Funcionalidades

- **Lurk Automático do Felipenor**:
  - Abre automaticamente o canal `twitch.tv/felipenor` quando entra ao vivo.
  - Se estiver offline, reproduz um vídeo específico em loop para manter o apoio.
- **Lista de Lurk Personalizada**: Adicione seus canais favoritos. Se eles entrarem ao vivo, a extensão abrirá uma aba mutada e fixada automaticamente.
- **Backup dos Favoritos**: Exporte seus canais favoritos para um arquivo `.json` e importe depois quando atualizar a extensão ou trocar de navegador.
- **Blacklist de Canais**: Bloqueie canais que você não quer que a extensão abra automaticamente. Se o alvo de uma raid estiver na blacklist, a guia é fechada.
- **Fechamento Opcional de Lives Encerradas**: No menu de configurações, você pode ativar o fechamento automático de guias quando a live termina e escolher se isso vale para todas as lives ou só para canais selecionados.
- **Conexão Oficial da Twitch**: Se quiser melhorar a verificação de lives, basta clicar em conectar com a Twitch no popup. A extensão cuida do restante sem exigir configuração técnica.
- **Coletor de Pontos**: Coleta automaticamente os baús de bônus de pontos de canal.
- **Downloader de Emotes**: Baixe qualquer emote (chat ou seletor) em alta qualidade segurando **ALT + Clique**.
- **Notificações Discord**: Configure um Webhook para receber avisos quando seus canais favoritos entrarem ao vivo.
- **Economia de Recursos**: Tenta reduzir a qualidade do vídeo automaticamente para economizar banda e processamento.
- **Recarga Opcional das Lives**: Permite recarregar automaticamente as lives abertas em um intervalo escolhido pelo usuário, com a opção desligada por padrão para não pesar o navegador.

## 📦 Como Baixar e Instalar

Como a extensão ainda não está na Chrome Web Store, você precisará instalá-la manualmente (modo desenvolvedor).

### Passo 1: Download

1. Baixe o arquivo `.zip` da extensão (disponibilizado nas Releases do GitHub ou pelo autor).
2. Extraia o conteúdo do arquivo `.zip` para uma pasta em seu computador (ex: `C:\ShadowLurk`).

### Passo 2: Instalação no Navegador

1. Abra seu navegador (Google Chrome, Edge, Brave, Opera GX).
2. Na barra de endereços, digite `chrome://extensions` e pressione Enter.
3. No canto superior direito, ative a chave **Modo do desenvolvedor** (Developer mode).
4. Clique no botão **Carregar sem compactação** (Load unpacked) que apareceu no canto superior esquerdo.
5. Selecione a pasta onde você extraiu os arquivos (a pasta que contém o arquivo `manifest.json`).

Pronto! A extensão ShadowLurk está instalada e ativa. O ícone deve aparecer na sua barra de ferramentas.

## 🔄 Como Atualizar Sem Perder os Favoritos

1. Antes de atualizar, abra o popup da extensão e clique em **Exportar favoritos**.
2. Salve o arquivo `.json` gerado em uma pasta segura no seu computador.
3. Atualize os arquivos da extensão no GitHub ou substitua a pasta local pela versão nova.
4. Abra `chrome://extensions` e clique em **Recarregar** na extensão ShadowLurk.
5. Abra o popup de novo e use **Importar favoritos** para restaurar sua lista personalizada.

Se você já estiver usando a mesma pasta da extensão no modo desenvolvedor, normalmente basta substituir os arquivos e clicar em **Recarregar** no painel de extensões do navegador.

## ⚙️ Como Usar

1. Clique no ícone da extensão para abrir o menu.
2. **Adicionar Canais**: Digite o nome do canal (ex: `gaules`, `alanzoka`) e clique em "Adicionar".
3. **Exportar / Importar Favoritos**: Use os botões abaixo da lista para salvar sua seleção em arquivo e restaurar depois de atualizar a extensão.
4. **Webhook Discord (Opcional)**: Cole a URL do seu Webhook do Discord para receber alertas.
5. **Twitch Oficial (Opcional)**: No popup, clique em **Conectar com a Twitch** se quiser ativar a verificação oficial e melhorar a detecção de lives.
6. **Recarga Automática (Opcional)**: No menu de configurações, ative a recarga automática e escolha o intervalo em minutos se quiser renovar as lives abertas periodicamente.
7. **AdBlock**: A extensão detecta se você está usando bloqueador de anúncios. Para apoiar os criadores, desative o AdBlock na Twitch.

**Lembre-se:** Deixe seu navegador aberto! A extensão verificará automaticamente a cada **1 minuto** se o Felipenor ou seus canais favoritos estão online.

## ❤️ Apoie o Criador

Esta extensão é totalmente gratuita, mas se você quiser apoiar o desenvolvimento e manutenção:

- **Twitch**: [twitch.tv/felipenor](https://twitch.tv/felipenor)
- **YouTube**: [youtube.com/@Felipenor](https://youtube.com/@Felipenor)
- **Doação (Pix)**: [livepix.gg/felipenor](https://livepix.gg/felipenor)
- **Doação (PayPal)**: [paypal.com/donate](https://www.paypal.com/donate?business=felipeczs41@gmail.com&currency_code=USD)

Desenvolvido com carinho por [**Felipenor**.](https://linkbio.co/felipenor)
