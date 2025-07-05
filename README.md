# MVP: Planejador de Viagens para Veículos Elétricos

Este projeto realiza uma análise da infraestrutura de pontos de recarga para veículos elétricos (VEs) no Brasil e culmina no desenvolvimento de uma ferramenta interativa para simular a viabilidade de rotas.

---

### Nota Importante Sobre a Visualização

Devido a componentes interativos e visualizações complexas (`folium`), o renderizador padrão do GitHub pode falhar ao tentar exibir este notebook, mostrando um erro de "Invalid Notebook". **Isso não é um erro no código.**

**Para visualizar e executar o projeto corretamente, por favor, abra o notebook diretamente no Google Colab usando o link abaixo:**

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/santana4884/MVP/blob/main/MVP.ipynb)
---

### Resultado Final da Simulação (Exemplo: São Paulo -> Rio de Janeiro)

Abaixo está um exemplo do mapa gerado pela ferramenta para a rota SP-RJ com um veículo de 300km de autonomia.

![Resultado do Mapa](https://github.com/santana4884/MVP/blob/main/Resultado_mapa.jpg?raw=true)

---

### Estrutura do Projeto

O notebook está organizado da seguinte forma:
1.  **Introdução e Definição do Problema:** Contextualização do desafio da "ansiedade de autonomia" e as hipóteses do projeto.
2.  **Setup Inicial:** Instalação e importação de bibliotecas e carregamento dos dados via API do Open Charge Map.
3.  **Análise Exploratória e Limpeza:** Análise da distribuição geográfica e padronização dos dados de estados.
4.  **Pré-processamento para Simulação:** Filtragem dos dados para obter apenas carregadores públicos e operacionais e a análise da rede de carregadores rápidos (DC).
5.  **Desenvolvimento do Planejador:** Implementação das funções de geocodificação, roteirização (via OpenRouteService) e a lógica de simulação de viagem.
6.  **Conclusão:** Resumo dos insights e validação das hipóteses.
