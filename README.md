# Automação de Notícias de Inteligência Artificial com Make e Google Sheets / AI News Automation with Make and Google Sheets

## Sobre o Projeto / About the Project
Este projeto consiste num fluxo de automação desenvolvido no Make para monitorizar e filtrar notícias de tecnologia e inteligência artificial de forma automatizada.

This project is an automation workflow developed in Make to monitor and filter technology and artificial intelligence news automatically.

## Como Funciona / How It Works
1. **Recolha (RSS Feed):** O sistema recolhe continuamente novos artigos a partir do feed oficial de notícias em `https://www.artificialintelligence-news.com/feed/`. / The system continuously collects new articles from the official news feed.
2. **Filtro Inteligente:** Aplica um filtro para verificar se a palavra "automação" está presente no título, na descrição ou no resumo da notícia. / It applies a filter to check if the word "automação" or "automation" is present in the title, description, or summary.
3. **Registo Automático (Google Sheets):** Caso a condição seja verdadeira, a linha é enviada para o Google Sheets com a seguinte estrutura: / If true, the row is sent to Google Sheets with the following structure:
   * **Coluna A / Column A:** Título da notícia / News title
   * **Coluna B / Column B:** Link direto para o artigo / Direct link to the article
   * **Coluna C / Column C:** Data de publicação ou atualização / Publication or update date
