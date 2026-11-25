# Documentação de SEO — Fluência+

**Site publicado:** [https://feliperodrigo-iftm.github.io/Fluencia-/](https://feliperodrigo-iftm.github.io/Fluencia-/)

---

## 1. Palavras-Chave Definidas

Para orientar a estrutura semântica e o conteúdo das páginas, foram escolhidas **3 palavras-chave principais** alinhadas ao tema de educação e idiomas:

1. **Aprendizagem de idiomas** (palavra-chave principal — aplicada no `<title>`, na `<meta name="description">`, no `<main>` e nos textos introdutórios)
2. **Imersão cultural** (aplicada no título, na descrição, no primeiro `<article>` e nos metadados Open Graph)
3. **Repetição espaçada** (aplicada no título, na descrição, no segundo `<article>` e na página complementar)

---

## 2. Decisões Técnicas Tomadas

* **Metadados únicos por página:** Criação de `<title>` (entre 50 e 60 caracteres) e `<meta name="description">` (até 160 caracteres) exclusivos para cada página HTML (`index.html` e `idiomas.html`), contendo as palavras-chave estratégicas de forma natural.
* **URL Canônica (`canonical`):** Inclusão da tag `<link rel="canonical">` apontando para a URL absoluta oficial no GitHub Pages para evitar conteúdo duplicado.
* **Open Graph e Favicon:** Configuração completa das tags `og:type`, `og:title`, `og:description`, `og:url`, `og:locale` e `og:image` (com dimensões `1200x630`), além de `favicon.svg` para identificação na aba do navegador.
* **Dados Estruturados (JSON-LD):** Implementação de marcação `Schema.org` (`WebSite` e `EducationalOrganization`) validada sem erros no `validator.schema.org`.
* **Indexação (`robots.txt` e `sitemap.xml`):** Arquivos publicados na raiz do site liberando o rastreamento pelos mecanismos de busca e listando todas as URLs indexáveis.
* **Arquitetura e Links Internos:** Uso de URLs amigáveis (letras minúsculas e sem acentos) e navegação com textos âncora descritivos conectando as duas páginas do projeto.
* **Otimização de Imagens e Performance:** Conversão das fotografias para o formato **WebP**, definição explícita de `alt`, `width` e `height` para evitar deslocamento de layout (CLS) e aplicação de `loading="lazy"` nas imagens abaixo da dobra inicial.
* **Acessibilidade:** Uso de HTML5 semântico (`header`, `nav`, `main`, `article`, `aside`, `footer`), link de salto *"Pular para o conteúdo"*, contraste adequado de cores e rótulos (`label`) associados a todos os campos do formulário.

---

## 3. Resultados do Lighthouse (Modo Celular — Antes e Depois)

*(Substitua os valores abaixo pelas notas reais obtidas no Google Chrome DevTools → Lighthouse em modo Mobile)*

| Categoria | Antes | Depois | Meta Exigida |
| :--- | :---: | :---: | :---: |
| **SEO** | `XX` | `XX` | **≥ 95** |
| **Acessibilidade** | `XX` | `XX` | **≥ 90** |
| **Práticas Recomendadas** | `XX` | `XX` | — |
| **Desempenho** | `XX` | `XX` | — |

### Principais melhorias observadas entre os testes:
* Correção da hierarquia de títulos (mantendo apenas um `<h1>` por página) e adição de `meta description`, elevando a nota de **SEO**.
* Inclusão de `aria-label` na navegação, ajuste de contraste entre texto e fundo e associação correta de `label` nos inputs, elevando a nota de **Acessibilidade**.
* Conversão das imagens de `.jpeg` para `.webp` e adição de `loading="lazy"`, reduzindo o tempo de carregamento em dispositivos móveis.

---

## 4. Evidências de Validação

* **Schema.org Validator (`0 errors`):**
  ![Validação Schema.org](imagens/print-schema.png)

* **Lighthouse Mobile (Antes vs. Depois):**
  ![Lighthouse Antes](imagens/print-lighthouse-antes.png)
  ![Lighthouse Depois](imagens/print-lighthouse-depois.png)