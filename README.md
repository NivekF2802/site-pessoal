# Site Pessoal & Portfólio — Kevin Bracht Fank

**Aluno:** Kevin Bracht Fank  
**Curso:** Bacharelado em Engenharia de Software  
**Instituição:** Universidade Tecnológica Federal do Paraná (UTFPR) — Câmpus Dois Vizinhos  
**Status do Projeto:** Etapa 2 Concluída (HTML5 Semântico + Metatags SEO/OG + CSS3 Responsivo + Modo Claro/Escuro)

---

## Objetivo do Projeto
Desenvolver incrementalmente um site pessoal e portfólio profissional aplicando os conceitos de **HTML5 semântico**, **metadados de identificação/compartilhamento** e **estilização avançada com CSS3 e Design Responsivo**, mantendo o histórico evolutivo no Git.

---

## Acesso ao Projeto
* **Deploy no GitHub Pages:** [https://nivekf2802.github.io/site-pessoal/](https://nivekf2802.github.io/site-pessoal/)
* **Repositório no GitHub:** [https://github.com/NivekF2802/site-pessoal](https://github.com/NivekF2802/site-pessoal)

---

## Destaques e Recursos Implementados

* **Identidade e Compartilhamento no `<head>`:**
  * **Favicon:** Ícone personalizado na aba do navegador.
  * **Meta Description:** Descrição otimizada para mecanismos de busca (SEO).
  * **Open Graph (OG) & Twitter Cards:** Metatags completas (`og:title`, `og:description`, `og:image`, `og:url`, `og:type` e `twitter:card`) para pré-visualização rica em redes sociais e apps de mensagem (WhatsApp, LinkedIn, X).
* **Sistema de Tema Claro / Escuro (Pure CSS):**
  * Alternância instantânea entre *Dark Mode* e *Light Mode* direto na barra de navegação utilizando variáveis CSS (`:root`) e seletor `:has()`, sem dependência de JavaScript.
* **Formato Landing Page & Slideshow Interativo:**
  * *Hero Section* com chamadas para ação (*CTAs*) e menu superior fixo (*sticky glassmorphism*).
  * Galeria rotativa de destaques no meio da página feita com CSS puro (`input[type="radio"]` + `transform: translateX`).
* **Design 100% Responsivo:**
  * Grade adaptável com CSS Grid, Flexbox e *Media Queries* para computadores, tablets e smartphones.

---

## Estrutura de Arquivos

```text
site-pessoal/
├── index.html        # Estrutura semântica, metatags (SEO/OG/Twitter) e conteúdo
├── style.css         # Folha de estilo externa com temas Claro/Escuro e responsividade
├── foto-kevin.jpg    # Imagem de perfil e pré-visualização Open Graph
└── README.md         # Documentação acadêmica do projeto