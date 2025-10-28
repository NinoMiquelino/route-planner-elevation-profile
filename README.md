## 👨‍💻 Autor

<div align="center">
  <img src="https://avatars.githubusercontent.com/ninomiquelino" width="100" height="100" style="border-radius: 50%">
  <br>
  <strong>Onivaldo Miquelino</strong>
  <br>
  <a href="https://github.com/ninomiquelino">@ninomiquelino</a>
</div>

---

# 🗺️ Planejador de Rotas Interativo com Perfil de Elevação

![JavaScript](https://img.shields.io/badge/Frontend-JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Layout-Bootstrap-563D7C?logo=bootstrap&logoColor=white)
![License MIT](https://img.shields.io/badge/License-MIT-green)
![Status Stable](https://img.shields.io/badge/Status-Stable-success)
![Version 1.0.0](https://img.shields.io/badge/Version-1.0.0-blue)
![GitHub stars](https://img.shields.io/github/stars/NinoMiquelino/route-planner-elevation-profile?style=social)
![GitHub forks](https://img.shields.io/github/forks/NinoMiquelino/route-planner-elevation-profile?style=social)
![GitHub issues](https://img.shields.io/github/issues/NinoMiquelino/route-planner-elevation-profile)

## Visão Geral

Este projeto é um Planejador de Rotas web interativo que permite aos usuários traçar uma rota clicando em vários pontos em um mapa. O aplicativo processa instantaneamente a rota, calculando a distância total e gerando um perfil de elevação simulado e realista.

É uma demonstração robusta de como integrar bibliotecas de mapeamento e visualização de dados para criar uma experiência geográfica rica em funcionalidades.

---

## 🚀 Habilidades e Tecnologias Demonstradas

Este projeto foi concebido para destacar as seguintes habilidades-chave em desenvolvimento Front-end e GIS (Geographic Information Systems):

| Habilidade | Descrição |
| :--- | :--- |
| **Traçado de Polylines Dinâmicas no Leaflet** | Uso de eventos de clique no mapa para adicionar pontos de rota em tempo real e atualizar o objeto `L.Polyline`. |
| **Cálculos Geográficos** | Implementação da **Fórmula de Haversine** para calcular a distância geodésica (real) acumulada entre os pontos da rota. |
| **Integração de Bibliotecas Externas** | Integração bem-sucedida do **Chart.js** para visualizar dados de elevação de forma profissional. |
| **Simulação de Dados** | Criação de uma lógica de `simulateElevation` que gera um perfil de elevação que se comporta de maneira realista (com subidas e descidas suaves). |
| **Manipulação de Eventos Complexos** | Gerenciamento de múltiplos eventos (clique, limpeza de rota) para atualizar o mapa, as métricas e o gráfico de forma síncrona. |

---

## ⚙️ Tecnologias Utilizadas

* **Leaflet.js:** Biblioteca de mapeamento Open-Source para renderização e interações no mapa.
* **Chart.js:** Biblioteca de gráficos simples e flexível para a visualização do perfil de elevação.
* **HTML/CSS:** Estrutura básica e estilização.
* **JavaScript (Vanilla JS):** Lógica principal, cálculos e manipulação de DOM.
* **Bootstrap (Opcional):** Para layout e design responsivo simples.

---

## 🧩 Estrutura do Projeto

```
route-planner-elevation-profile/
├── index.html
├── README.md
├── .gitignore
└── LICENSE
```

---

## 🛠️ Como Usar

Para testar o projeto:

1.  **Clone o repositório** (ou copie o código se for um único arquivo).
2.  **Salve o código** em um arquivo chamado `index.html`.
3.  **Abra o arquivo** `index.html` em seu navegador.
4.  **Clique no mapa** em diferentes localizações para traçar sua rota.

A cada clique, a distância total será atualizada e o gráfico de perfil de elevação abaixo do mapa será redesenhado instantaneamente.

---

## 🧠 Lógica Chave do Projeto

A funcionalidade central reside em três etapas no evento de clique (`onMapClick`):

1.  **Registro do Ponto:** As coordenadas (`latlng`) são armazenadas no array `routePoints` e um novo marcador é adicionado ao mapa.
2.  **Cálculo:** A função `updateRouteMetrics` calcula a distância total usando a Fórmula de Haversine e, em seguida, chama `simulateElevation`.
3.  **Visualização:** A função `simulateElevation` gera o array de dados `[distância, elevação]`, que é então passado para a função `updateChart` para redesenhar o gráfico do Chart.js.

---

## 🤝 Contribuições
Contribuições são sempre bem-vindas!  
Sinta-se à vontade para abrir uma [*issue*](https://github.com/NinoMiquelino/route-planner-elevation-profile/issues) com sugestões ou enviar um [*pull request*](https://github.com/NinoMiquelino/route-planner-elevation-profile/pulls) com melhorias.

---

## 💬 Contato
📧 [Entre em contato pelo LinkedIn](https://www.linkedin.com/in/onivaldomiquelino/)  
💻 Desenvolvido por **Onivaldo Miquelino**

---
