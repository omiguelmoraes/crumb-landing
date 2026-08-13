# Crumb — landing

Landing de waitlist do [Crumb](https://crumb-omiguelmoraes-6275s-projects.vercel.app),
app de bookmarks focado em **recuperação**, não em armazenamento.

> Você já salvou. O problema é reencontrar.

HTML estático, sem build. `index.html` carrega tudo — estilo, motor de busca e demo.

## A demo é real

A seção "Lembra torto. Ele entende." roda o motor de busca de verdade na página.
Ele quebra a frase em cor + tipo + época + termo livre, e cada resultado mostra
por que apareceu. Não é vídeo nem GIF.

## Waitlist

A constante `FORM_ENDPOINT` no topo do script está vazia. Enquanto estiver assim,
o formulário guarda em `localStorage` e só confirma na tela. Para coletar de verdade,
cole a URL do Formspree (ou Resend/Buttondown) ali.

## Marca

| Token | Valor |
| --- | --- |
| Papel | `#FFF3EA` |
| Tinta | `#14100D` |
| Laranja | `#FF5C00` |
| Display | Schibsted Grotesk 300 |
| Corpo | Geist |

O laranja é acento — botão e símbolo. Nunca fundo de área grande, nunca palavra
colorida no título.

## Deploy

Conectado ao GitHub: push na `main` dispara deploy de produção automaticamente.
Para subir manualmente:

```bash
vercel deploy --prod
```

Ao trocar de domínio, atualizar as URLs absolutas de `og:image`, `og:url` e `canonical`
no `<head>` — LinkedIn e WhatsApp não aceitam caminho relativo.
