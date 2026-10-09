# motoTX — aplicativo instalável para celular

Aplicativo web instalável (PWA) para o cliente marcar a localização pelo GPS, conferir o ponto no mapa e abrir uma conversa no WhatsApp **+55 86 99579-9484** com o link do Google Maps.

## Como funciona
1. O cliente abre o motoTX pelo navegador do celular.
2. Toca em **Marcar minha localização** e permite o acesso à localização.
3. O mapa centraliza no GPS e mostra um marcador.
4. Toca em **Enviar localização pelo WhatsApp**.
5. O WhatsApp abre a conversa com a mensagem pronta. O cliente ainda precisa tocar em **Enviar** no WhatsApp.

## Publicar com HTTPS
A localização GPS normalmente só funciona em contexto seguro (HTTPS), exceto localhost. Publique estes arquivos em um serviço de hospedagem estática com HTTPS, como GitHub Pages, Netlify ou Render Static Site.

### GitHub Pages (resumo)
1. Crie um repositório chamado `mototx`.
2. Envie todos os arquivos desta pasta para a raiz do repositório.
3. Em **Settings → Pages**, escolha a publicação a partir da branch principal e da pasta `/ (root)`.
4. Aguarde a URL HTTPS ser criada e abra-a no celular.

## Instalar no Android
1. Abra a URL HTTPS no Chrome do Android.
2. Abra o menu ⋮ e toque em **Instalar app** ou **Adicionar à tela inicial**.
3. Abra o motoTX pelo ícone criado.

## Observações
- O mapa usa OpenStreetMap via Leaflet e precisa de internet para carregar os mapas.
- A localização é solicitada somente quando o cliente toca no botão.
- O aplicativo não envia mensagens silenciosamente; ele abre o WhatsApp com o texto preenchido e o cliente confirma o envio.
- Para usar a geolocalização, permita a localização no navegador e ative o GPS do aparelho.
- O service worker guarda os arquivos básicos para facilitar a abertura posterior, mas mapas e WhatsApp continuam dependendo da internet.
