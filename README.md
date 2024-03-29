# Bot ImóveisFinder

Este é um bot desenvolvido em Node.js para encontrar e-mails em páginas de imóveis em vários sites de imobiliárias e classificados.

## Descrição

O `ImóveisFinder` é um bot construído com Node.js que utiliza técnicas de web scraping para percorrer páginas de diversos sites imobiliários em busca de informações de contato (e-mails) presentes nessas páginas. Ele é projetado para encontrar e-mails associados a listagens de imóveis em várias plataformas, agregando essa informação em um banco de dados MongoDB e salvando também em um arquivo de texto.

## Funcionamento

### Arquivos Principais:

- `app.js`: Contém a lógica principal do bot, onde se estabelece a conexão com o MongoDB e a função de busca e salvamento de e-mails.
- `webScraper.js`: Contém a lógica de web scraping para rastrear as páginas dos sites de imóveis e encontrar e-mails.

### Tecnologias Utilizadas:

- `axios`: Utilizado para fazer requisições HTTP para as páginas web.
- `cheerio`: Uma biblioteca para analisar e manipular HTML e XML.
- `fs`: Módulo de sistema de arquivos Node.js.
- `mongoose`: Biblioteca para modelar objetos no MongoDB.

### Uso:

O bot utiliza um intervalo de 24 horas para executar a busca de e-mails nos sites listados em `webScraper.js` e armazena os e-mails encontrados no banco de dados MongoDB. Além disso, salva esses e-mails em um arquivo de texto local chamado `email.txt`.

## Instalação e Uso

1. Certifique-se de ter o Node.js instalado na sua máquina.
2. Clone o repositório.
3. Execute `npm install` para instalar as dependências.
4. Configure a conexão com o MongoDB no arquivo `app.js`.
5. Execute o bot com `node app.js`.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para enviar pull requests ou sugestões.

## Autor

- Bruno Ribeiro

## Licença

Este projeto está sob a MIT.
