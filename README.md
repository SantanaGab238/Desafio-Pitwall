# 🏎️ Desafio Pit Wall — GP de São Paulo de F1

Um projeto web front-end que reproduz a página oficial do **GP de São Paulo de F1**, desenvolvido exclusivamente com **HTML5** e **CSS3** como parte da disciplina de **Linguagem de Marcação (LIMA)**.

---

## 📌 Sobre o Projeto

O **Desafio Pit Wall** tem como objetivo aplicar os conceitos de estruturação HTML, estilização CSS, layouts dinâmicos e responsividade aprendidos ao longo das aulas. A proposta consiste em recriar a interface visual de transmissão e reserva de ingressos para o GP de São Paulo, garantindo uma adaptação perfeita para ecrãs de computadores e dispositivos móveis.

* **Professores:** André Denani e Raul Lopes
* **Disciplina:** Linguagem de Marcação (LIMA)
* **Escopo:** Front-End estático (sem scripts JS ou integração backend)

---

## 🛠️ Tecnologias e Conceitos Aplicados

| Conceito / Recurso | Aplicação no Projeto | O que foi treinado |
| :--- | :--- | :--- |
| `:root` e `var()` | Cores da paleta principal (`--black`, `--panel`, `--red`, `--white`) e variáveis de equipas | Organização e reaproveitamento de estilos |
| `Flexbox` | Barra de topo (`topbar`), navegação do menu, estatísticas da pista e filtros | Alinhamento e distribuição unidimensional |
| `CSS Grid` | Grelha de cards dos pilotos (`repeat(auto-fit, minmax(220px, 1fr))`) | Layouts bidimensionais automáticos |
| `Form Grid` | Formulário de reserva de ingressos em 2 colunas com a classe `.full` | Estruturação e alinhamento de formulários |
| `Tabelas HTML` | Tabela de classificação (`<table>`, `<thead>`, `<tbody>`) | Exibição de dados tabulares estruturados |
| Responsividade (`@media`) | Adaptação para ecrãs móveis (até 768px) | Media Queries e reorganização de conteúdos |
| Fontes Externas | Google Fonts (*Titillium Web*) | Importação e aplicação de tipografia |
| Efeitos Visuais | Corte seco com `linear-gradient`, zebra de pista com `repeating-linear-gradient`, `opacity`, `hover` e `transform` | Estilização avançada e transições suaves |

---

## 📐 Estrutura das Secções

A página é composta por 6 blocos principais de conteúdo:

1. **`header.topbar`**: Logótipo com destaque, menu de navegação e botão de ação em Flexbox.
2. **`section.hero` + `div.kerb`**: Título de grande dimensão, dados da pista, imagem de fundo com degradê inclinado (`piloto.jpg`) e a zebra de pista com gradiente repetitivo.
3. **`section#pilotos`**: Grelha de cards com números em marca de água e cores personalizadas por equipa.
4. **`section#classificacao`**: Filtros de pesquisa e tabela completa de pontuação do campeonato.
5. **`section#ingressos`**: Layout em 2 colunas contendo informações de setores à esquerda e o formulário de reserva à direita.
6. **`footer`**: Rodapé informativo centralizado.

> ℹ️ As secções `#pilotos`, `#classificacao` e `#ingressos` encontram-se agrupadas dentro da tag `<main class="container">`.

---

## 📂 Estrutura de Ficheiros

```text
pit-wall/
├── index.html     # Estrutura e conteúdo da página
├── styles.css     # Estilos, variáveis e regras de responsividade
└── img/           # Diretório de recursos visuais
    └── piloto.jpg # Imagem de fundo da secção Hero
