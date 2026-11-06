# Meu plano alimentar (PWA)

Conteúdo: `index.html`, `manifest.webmanifest`, `sw.js` (funciona offline) e a pasta `icons/`.

## Como publicar (precisa de HTTPS)
Suba a pasta inteira, mantendo os arquivos juntos na raiz do site. Opções gratuitas: Netlify Drop (app.netlify.com/drop), Cloudflare Pages ou GitHub Pages.

### Tirar a marca "Powered by Netlify"
No Netlify, abra o projeto e vá em Project configuration > General > Powered by Netlify badge e desative. A marca vem da plataforma, não do app.

## Como instalar no celular
- Android (Chrome): abra o endereço e toque em Instalar app.
- iPhone (Safari): Compartilhar, depois Adicionar à Tela de Início.

## Como o plano é carregado
Na primeira abertura, a pessoa toca em Copiar instruções, cola em um assistente de IA (ChatGPT, Claude etc.) junto com as fotos, o PDF ou o texto do plano e cola a resposta no app. Não precisa de servidor.

## Atualizações
Ao mudar o `index.html`, altere também a versão em `sw.js` (`const V`) para os celulares receberem a novidade.
Os registros ficam no aparelho (localStorage). Peça aos usuários para fazer backup de vez em quando.
