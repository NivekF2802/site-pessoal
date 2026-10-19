# Portfólio & Site Pessoal — Kevin Bracht Fank

**Aluno:** Kevin Bracht Fank  
**Curso:** Bacharelado em Engenharia de Software  
**Instituição:** Universidade Tecnológica Federal do Paraná (UTFPR) — Câmpus Dois Vizinhos  
**Status do Projeto:** Concluído (Etapas 1, 2 e 3 integradas)

---

## Links de Acesso e Validação

- **Site Publicado (GitHub Pages):** [https://nivekf2802.github.io/site-pessoal/](https://nivekf2802.github.io/site-pessoal/)
- **Repositório (Código-Fonte):** [https://github.com/NivekF2802/site-pessoal](https://github.com/NivekF2802/site-pessoal)

---

## Objetivo Geral

Desenvolver um site pessoal e portfólio profissional de forma incremental ao longo das aulas, mantendo o histórico de evolução no mesmo repositório Git. O projeto avança desde a marcação estrutural pura em HTML5, passando pela estilização visual desacoplada em CSS3, até a reconstrução responsiva sob a arquitetura **Mobile First** utilizando **Flexbox** e **CSS Grid**.

---

## Etapas Desenvolvidas

### 1. Site pessoal com HTML puro
Na primeira etapa, o foco exclusivo foi o domínio da linguagem de marcação e a estruturação semântica do conteúdo, sem utilização de CSS ou JavaScript:
- **Estrutura Básica e Semântica W3C:** Uso adequado de `<!DOCTYPE html>`, `<html lang="pt-BR">`, `<head>`, `<body>`, `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>` e `<footer>`.
- **Seções Obrigatórias e Conteúdo:**
  - Nome, título profissional e apresentação inicial.
  - Imagem representativa de perfil (`<figure>`, `<img>` com atributo `alt` e `<figcaption>`).
  - Seção **Sobre Mim** (trajetória do IFSC à UTFPR, atuação na Prothera e objetivos).
  - Seção de **Experiência Profissional** e **Formação Acadêmica**.
  - Seção de **Tecnologias & Habilidades** e **Projetos & Áreas de Foco**.
  - Seção de **Perfis e Conexões** com hyperlinks externos seguros (`target="_blank"` e `rel="noopener noreferrer"`) para GitHub e LinkedIn.
- **Navegação Interna:** Menu de navegação com âncoras funcionais (`#sobre-mim`, `#experiencia`, `#formacao`, `#tecnologias`, `#projetos`, `#perfis`, `#contato`) e link de retorno ao topo.
- **Área de Contato:** Formulário estruturado com `<form>`, `<label>`, `<input>` (`text`, `email`), `<textarea>`, validações nativas (`required`) e botões de envio/limpeza (`submit` e `reset`).
- **Metadados e Identidade no `<head>`:**
  - **Favicon:** Ícone vetorial em SVG com as iniciais `KF` e fallback `favicon.ico`.
  - **SEO:** `meta description` e `meta author`.
  - **Open Graph (OG) & Twitter Cards:** Metatags configuradas (`og:title`, `og:description`, `og:image`, `og:url`, `og:type` e `twitter:card`) para pré-visualização rica ao compartilhar o link no WhatsApp, LinkedIn e X.

---

### 2. Site pessoal com CSS
Na segunda etapa, a apresentação visual foi totalmente separada da estrutura HTML por meio de uma folha de estilos externa (`style.css`):
- **Design System com Variáveis CSS (`:root`):** Padronização de cores, tipografia, espaçamentos, bordas arredondadas (`border-radius`), sombras (`box-shadow`) e transições suaves.
- **Sistema de Tema Claro / Escuro (Pure CSS):** Alternador interativo na barra de navegação utilizando `<input type="checkbox">` oculto combinado ao seletor `:has(#theme-toggle:checked)`, permitindo alternar entre *Dark Mode* e *Light Mode* sem JavaScript.
- **Formato Landing Page:**
  - Cabeçalho com efeito translúcido (*backdrop-filter: blur*).
  - *Hero Section* de abertura com selo de status (*badge*), chamada de destaque, moldura estilizada na foto de perfil e botões de ação (*Call to Action*).
  - Linha do tempo (*timeline*) visual para as experiências profissionais.
- **Slideshow Interativo no Meio da Página (Pure CSS):** Galeria rotativa de destaques técnicos construída com controles `input[type="radio"]`, seletores de irmãos (`~`) e deslocamento horizontal via `transform: translateX()`, controlada por indicadores clicáveis (*bullets*).
- **Microinterações e Estados:** Estilização de estados `:hover` em cartões, botões e links, além de realce acessível `:focus` nos campos do formulário.

---

### 3. Site pessoal Mobile First com Layout Flexível ou em Grade
Na terceira etapa, o CSS foi reconstruído seguindo a estratégia **Mobile First**, onde o código base representa a experiência otimizada para telas pequenas e as adaptações para telas maiores são adicionadas progressivamente com *Media Queries* (`min-width`):
- **Configuração e Fluidez:**
  - Viewport configurado (`<meta name="viewport" content="width=device-width, initial-scale=1.0">`).
  - Eliminação de larguras fixas incompatíveis; adoção de unidades relativas e fluidas (`%`, `rem`, `fr`, `clamp()`).
  - Garantia de contenção de mídia com `max-width: 100%` e `height: auto`.
- **Versão Base — Mobile (~375px):**
  - Empilhamento vertical em coluna única (`grid-template-columns: 1fr` e `flex-direction: column`).
  - Na *Hero Section*, a foto é exibida acima do texto (`flex-direction: column-reverse`) com alinhamento centralizado.
  - Botões de ação e campos de formulário ocupam `100%` da largura útil para facilitar o toque em dispositivos móveis.
- **Breakpoint Tablet — `@media (min-width: 768px)`:**
  - Ativação do cabeçalho fixo no topo (`position: sticky`).
  - Conversão das grades de Sobre Mim, Formação, Tecnologias, Projetos, Perfis e linhas de Nome/E-mail do formulário para **2 colunas** (`grid-template-columns: repeat(2, 1fr)`).
  - Alinhamento horizontal de botões e do rodapé com **Flexbox**.
- **Breakpoint Desktop — `@media (min-width: 1200px)`:**
  - Barra de navegação distribuída horizontalmente em linha única (`justify-content: space-between`).
  - *Hero Section* disposta em duas colunas lado a lado (`flex-direction: row`), com apresentação textual alinhada à esquerda e foto à direita.
  - Expansão da seção de Tecnologias & Habilidades para **4 colunas** (`grid-template-columns: repeat(4, 1fr)`).

---

## Validação de Responsividade (DevTools)

O layout foi testado e validado nas três larguras de referência do navegador:
1. **Mobile (~375px):** Layout em 1 coluna, menu compacto centralizado, imagem redimensionada (`180px`) e botões com largura total.
2. **Tablet (~768px):** Cabeçalho *sticky*, cartões e campos superiores do formulário organizados em grade de 2 colunas.
3. **Desktop (>= 1200px):** Container amplo (`max-width: 1140px`), *Hero Section* lado a lado e grade de tecnologias em 4 colunas.

---

## Estrutura de Arquivos do Repositório

- `index.html` — Estrutura semântica HTML5, metadados SEO/OG/Twitter, controles de tema e slideshow.
- `style.css` — Estilização Mobile First, variáveis de tema Claro/Escuro, Flexbox, CSS Grid e Media Queries.
- `foto-kevin.jpg` — Imagem representativa de perfil e pré-visualização de compartilhamento.
- `README.md` — Documentação completa das três etapas da atividade.