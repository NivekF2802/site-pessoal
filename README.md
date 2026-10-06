# Site Pessoal - Etapa 1: Estruturação com HTML Puro

**Aluno:** Kevin Bracht Fank  
**Curso:** Bacharelado em Engenharia de Software  
**Instituição:** Universidade Tecnológica Federal do Paraná (UTFPR) - Câmpus Dois Vizinhos  
**Status do Projeto:** Etapa 1 Concluída (HTML5 Semântico Puro)

---

## Objetivo da Atividade
Desenvolver a primeira versão incremental de um site pessoal utilizando unicamente **HTML5**, sem qualquer regra de estilo CSS, bibliotecas auxiliares ou JavaScript. 

O foco central desta etapa é evidenciar o domínio da linguagem de marcação como esqueleto fundamental da web, priorizando:
- Estruturação semântica formal (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`).
- Hierarquia lógica de títulos (`<h1>` a `<h3>`).
- Navegação interna por âncoras funcionais.
- Acessibilidade básica e legibilidade de formulário para coleta de dados via `<form>`.
- Preparação da base estrutural para posterior adição de CSS e responsividade nas próximas aulas.

---

## Link do Site Publicado
- **GitHub Pages:** [Acesse o site publicado aqui](https://nivekf2802.github.io/site-pessoal/)

---

## Arquivos do Repositório
- `index.html`: Código-fonte com a marcação completa do site.
- `foto-kevin.jpg`: Imagem representativa de perfil utilizada na página.
- `README.md`: Identificação acadêmica, objetivos e link de validação.

# Site Pessoal & Portfólio — Etapa 2: Estilização com CSS3 e Design Responsivo

**Aluno:** Kevin Bracht Fank  
**Curso:** Bacharelado em Engenharia de Software  
**Instituição:** Universidade Tecnológica Federal do Paraná (UTFPR) — Câmpus Dois Vizinhos  
**Status do Projeto:** Etapa 2 Concluída (HTML5 Semântico + CSS3 Externo + Design Responsivo)

---

## Objetivo da Atividade
Evoluir o repositório do site pessoal separando rigorosamente a **estrutura e conteúdo** (HTML5) da **apresentação visual** (CSS3). 

Nesta etapa, o projeto foi transformado em formato de **Landing Page moderna**, incorporando as sugestões apontadas pelo professor:
1. **Estrutura de Landing Page:** Inclusão de *Hero Section* com botões de chamada para ação (*CTA*), apresentação destacada, status de atuação e barra de navegação superior com efeito fosco (*glassmorphism*).
2. **Slideshow no Meio da Página:** Implementação de uma galeria/slideshow interativa no meio do documento construída exclusivamente com **CSS puro** (utilizando a técnica de `radio buttons` ocultos e pseudo-classes `:checked`), sem dependência de JavaScript.
3. **Design Responsivo & Mobile Friendly:** Layout fluído adaptado para computadores, tablets e smartphones por meio de *Media Queries*, CSS Grid e Flexbox.

---

## Acesso ao Projeto
* **Deploy no GitHub Pages:** [https://nivekf2802.github.io/site-pessoal/](https://nivekf2802.github.io/site-pessoal/)
* **Repositório no GitHub:** [https://github.com/NivekF2802/site-pessoal](https://github.com/NivekF2802/site-pessoal)

---

## Tecnologias e Recursos CSS Aplicados

* **Folha de Estilos Externa (`style.css`):** Desacoplamento total de estilos do documento HTML.
* **Design System & Variáveis CSS (`:root`):**
  * Paleta de cores temática *Dark Tech* (`#0b1120`, `#131c31`, `#2563eb`, `#38bdf8`).
  * Tipografia padronizada e hierarquia visual clara (`font-size`, `line-height`, `letter-spacing`).
  * Espaçamentos sistemáticos, cantos arredondados (`border-radius`) e elevação com sombras (`box-shadow`).
* **Layout Moderno (Flexbox & CSS Grid):**
  * Alinhamento e distribuição da barra de navegação e *Hero Section* com Flexbox.
  * Disposição adaptável em colunas para formações, tecnologias, projetos e perfis utilizando `grid-template-columns: repeat(auto-fit, minmax(...))`.
* **Microinterações e Estados Interativos:**
  * Efeitos suaves de transição (`transition`) e hover em links, botões e cartões de projeto (`transform: translateY(-2px)`).
  * Estados de foco (`:focus`) visíveis e acessíveis em todos os campos do formulário de contato.
* **Slideshow Interativo (Pure CSS):**
  * Transição horizontal controlada via seletores de irmãos adjacentes (`~`) e `transform: translateX()`.
  * Navegação por marcadores clicáveis (*bullets*).
* **Media Queries & Responsividade:**
  * Breakpoints definidos em `900px` e `768px` para reorganização de fluxos, ajustes tipográficos e adaptação da grade para dispositivos móveis.

---

## 📁 Estrutura de Arquivos

```text
site-pessoal/
├── index.html        # Estrutura semântica e conteúdo do site
├── style.css         # Folha de estilo externa com regras de layout e design responsivo
├── foto-kevin.jpg    # Imagem de perfil otimizada
└── README.md         # Documentação da entrega e registro das etapas