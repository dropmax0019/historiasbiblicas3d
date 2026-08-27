EBD 3D — Landing Page final com tracking

Antes de publicar, abra index.html e preencha o objeto window.EBD_CONFIG no início do <head>:
- metaPixelId: ID do Pixel da Meta usado na sua conta
- checkoutBasic: URL da oferta Wiapy de R$10,00
- checkoutComplete: URL da oferta Wiapy de R$27,67
- checkoutUpgrade: URL da oferta especial Wiapy de R$17,89

Tracking:
- A landing captura utm_source, utm_medium, utm_campaign, utm_content, utm_term e fbclid da URL do anúncio.
- Esses parâmetros são preservados e adicionados automaticamente aos links dos três checkouts.
- A landing dispara PageView e ViewContent quando o Meta Pixel estiver configurado.
- NÃO dispara InitiateCheckout no clique do botão. Conforme solicitado, esse evento deve acontecer no ambiente do checkout/Wiapy quando o checkout for efetivamente aberto.
- A compra (Purchase) deve continuar sendo enviada pela integração Meta da Wiapy.

Importante:
- Não coloque um Purchase manual na landing.
- Não duplique o Pixel da Meta.
- Teste os três fluxos e valide os eventos no Meta Events Manager antes de iniciar tráfego.
