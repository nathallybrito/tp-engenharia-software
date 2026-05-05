# Textalyzer: Analisador de Texto para Planilha

## 1. Membros do Grupo
* Gustavo Henrique
* Lucas Cassio
* Náthally Fernandes
* Rafael Chimicatti

## 2. Explicação do Sistema
O **Textalyzer** é uma aplicação de linha de comando (CLI) projetada para receber um bloco de texto (via input ou arquivo `.txt`) e processá-lo para gerar uma planilha de dados (no formato `.csv`). O sistema processa a entrada e extrai estatísticas úteis, como:
* Contagem total de palavras e caracteres.
* Frequência de ocorrência de cada palavra.
* Tamanho médio das palavras.

**Foco em Qualidade e Manutenção (Objetivo do TP):**
O sistema foi arquitetado de forma modular, separando a lógica de negócio (análise do texto) da lógica de infraestrutura (leitura/escrita de arquivos). O principal objetivo desta arquitetura é facilitar a implementação de testes automatizados. Através da nossa suíte de testes, buscaremos evidenciar como a cobertura de código previne regressões — garantindo que a adição de novas métricas de texto ou a alteração do formato da planilha no futuro não quebre as funcionalidades já existentes.

## 3. Tecnologias Utilizadas
* **Python:** Linguagem de programação escolhida para o desenvolvimento do sistema, devido à sua facilidade na manipulação de *strings* e suporte nativo a arquivos de dados.
* **Módulo `csv`:** Biblioteca padrão do Python utilizada para a geração e exportação da planilha.
* **Pytest:** Framework utilizado para a criação e execução dos testes unitários. Ele será responsável por validar o comportamento das funções de análise (ex: *fixtures* para diferentes cenários de entrada de texto).
* **GitHub Actions (CI):** Utilizado para configurar um fluxo de Integração Contínua (Continuous Integration). A cada *commit* ou *pull request* submetido ao repositório, os testes serão executados automaticamente, demonstrando na prática como a automação auxilia na manutenção da saúde do software.
