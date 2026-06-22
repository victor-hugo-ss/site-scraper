# site-scraper

Um scraper simples que usa Puppeteer e Cheerio para coletar títulos e URLs de livros (ex.: categoria Science Fiction em books.toscrape.com).

## Requisitos

- Node.js (>= 18)
- npm ou yarn
- Acesso à internet para o Puppeteer abrir páginas

## Instalação

1. Instalar dependências:

   npm install

2. (Opcional) Instalar navegadores gerenciados pelo Puppeteer:

   npm run install-browser

## Uso

Executar o scraper:

npm start

ou

node ./src/index.js

O script percorre os elementos `article` da página alvo e imprime no console o título do livro e a URL.

## Scripts úteis (package.json)

- `start` — roda `node ./src/index.js`
- `install-browser` — instala navegadores utilizados pelo Puppeteer (`puppeteer browsers install chrome`)

## Observações e solução de problemas

- Arquivo de entrada: `src/index.js` (definido como `main` em package.json).
- Se ocorrerem erros relacionados ao navegador, rode `npm run install-browser` e verifique se o Puppeteer está permitido a abrir janelas no seu ambiente.

## Exemplo de saída

"A Light in the Attic" https://books.toscrape.com/catalogue/some-book-url

## Licença

MIT

## Autor

victor-hugo-ss <victorabreu2512@gmail.com>
