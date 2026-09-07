# Automações com Make / Make Automations

## Sobre o Repositório / About the Repository
Este repositório reúne os meus projetos, fluxos e exercícios práticos desenvolvidos na plataforma de automação **Make**.

This repository contains my projects, workflows, and practical exercises developed on the **Make** automation platform.

# 1. Integração de Meteorologia com Router e Filtros / Weather Integration with Router and Filters

## Resumo / Summary
* **PT:** Automação que recolhe dados meteorológicos em tempo real, utiliza um Router para dividir o fluxo de dados e aplica filtros lógicos avançados com base na temperatura para organizar automaticamente a informação em folhas de cálculo separadas no Google Sheets.
* **EN:** Automation that collects real-time weather data, uses a Router to split the data flow, and applies advanced logical filters based on temperature to automatically organize information into separate spreadsheets in Google Sheets.

## Sobre o Projeto / About the Project

* **PT:**
  * **Módulo Weather (Gatilho):** Funciona como o ponto de partida do cenário, encarregando-se de extrair e recolher periodicamente os dados meteorológicos atuais da localização pretendida.
  * **Módulo Router (Divisor):** Atua como o centro de controlo do fluxo, recebendo os dados recolhidos pelo módulo anterior e dividindo a rota principal em caminhos paralelos independentes.
  * **Filtros com Lógica Condicional (Filtros de Temperatura e Regras AND/OR):** Funcionam como barreiras seletivas em cada ramificação do Router, aplicando regras matemáticas e operadores lógicos estritos (como separar os dados em função de limiares de temperatura específicos, por exemplo, acima ou abaixo de 20 graus).
  * **Módulo Google Sheets (Ação Final):** Representa o destino final dos dados em cada caminho, sendo responsável por adicionar de forma limpa e estruturada uma nova linha na folha de cálculo correspondente, garantindo que os registos ficam devidamente catalogados consoante a regra cumprida.

* **EN:**
  * **Weather Module (Trigger):** Acts as the starting point of the scenario, responsible for extracting and periodically retrieving current meteorological data for the target location.
  * **Router Module (Splitter):** Serves as the flow control center, receiving the data retrieved by the previous module and splitting the main route into independent parallel paths.
  * **Filters with Conditional Logic (Temperature Filters and AND/OR Rules):** Act as selective barriers on each branch of the Router, applying strict mathematical rules and logical operators (such as separating data based on specific temperature thresholds, e.g., above or below 20 degrees).
  * **Google Sheets Module (Final Action):** Represents the final destination of data along each path, responsible for cleanly and structurally appending a new row to the corresponding spreadsheet, ensuring records are properly categorized according to the met rule.
  ![Make Foundation Metereologia](./Make%20Foundation%20-%20Metereologia.png)
 
    # 2. Filtro de Notícias por RSS / RSS News Filter Automation

## Resumo / Summary
* **PT:** Automação que recolhe continuamente artigos através de um feed RSS, aplica um filtro inteligente focado na palavra-chave "Automação" para selecionar apenas conteúdo relevante e regista automaticamente os dados estruturados no Google Sheets.
* **EN:** Automation that continuously collects articles via an RSS feed, applies an intelligent filter focused on the keyword "Automação" to select only relevant content, and automatically records structured data into Google Sheets.

## Esquema do Fluxo / Workflow Scheme

## Sobre o Projeto / About the Project

* **PT:**
  * **Módulo RSS (Gatilho):** Funciona como o ponto de partida do cenário, encarregando-se de extrair e monitorizar continuamente novos itens e artigos publicados através do feed RSS configurado.
  * **Filtro Inteligente (Filtragem por Palavra-Chave):** Atua como uma barreira seletiva logo após a recolha, aplicando uma condição baseada numa palavra-chave específica (neste caso, "Automação") para garantir que apenas os artigos estritamente relevantes avançam no fluxo.
  * **Módulo Google Sheets (Ação Final):** Representa o destino final dos dados filtrados, sendo responsável por adicionar de forma limpa e estruturada uma nova linha com informações como o título, a data e a hiperligação da notícia respetiva.

* **EN:**
  * **RSS Module (Trigger):** Acts as the starting point of the scenario, responsible for extracting and continuously monitoring new items and articles published through the configured RSS feed.
  * **Intelligent Filter (Keyword Filtering):** Acts as a selective barrier right after collection, applying a condition based on a specific keyword (in this case, "Automação") to ensure only strictly relevant articles move forward in the workflow.
  * **Google Sheets Module (Final Action):** Represents the final destination of the filtered data, responsible for cleanly and structurally appending a new row with information such as the title, date, and link of the respective news article.
 
    ![RSS Notícias](./RSS%20not%C3%ADcias.png)
