# 📚 Estudos HTML, CSS e JavaScript

Repositório dedicado ao aprendizado dos fundamentos do desenvolvimento web, incluindo HTML, CSS e JavaScript.

## 🚀 Objetivo

Construir uma base sólida em:
- Estrutura HTML
- Semântica
- Organização de código
- Boas práticas de desenvolvimento web

---

## 🧱 Estrutura básica do HTML

Todo arquivo HTML segue uma estrutura padrão. Pense como uma casa:

- Fundação → `<!DOCTYPE html>`
- Estrutura → `<html>`
- Configurações → `<head>`
- Conteúdo → `<body>`

### Exemplo:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Minha Página</title>
</head>
<body>
  <h1>Olá mundo</h1>
</body>
</html>
```

---

## ⚙️ Função das principais tags

| Tag/Atributo        | Função |
|---------------------|--------|
| `<!DOCTYPE html>`   | Define o HTML5 |
| `lang="pt-BR"`      | Define o idioma da página |
| `charset="UTF-8"`   | Suporte a acentos |
| `viewport`          | Responsividade |
| `<title>`           | Nome da aba do navegador |

---

## 📌 Pontos importantes

- Sem `UTF-8`, caracteres especiais quebram  
- `viewport` é essencial para mobile  
- `lang` melhora acessibilidade  
- `<head>` → configurações  
- `<body>` → conteúdo visível  

---

## 🧠 HTML semântico vs não semântico

### ❌ Não semântico (div soup)

```html
<div class="header">
  <div class="nav"></div>
</div>
```

### ✅ Semântico

```html
<header>
  <nav></nav>
</header>
```

---

## 🏗️ Exemplo de layout semântico

```html
<body>
  <header>
    <h1>Nome do Site</h1>
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/sobre">Sobre</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <article>
      <h2>Título do artigo</h2>
      <p>Conteúdo...</p>
    </article>

    <aside>
      <h3>Relacionados</h3>
    </aside>
  </main>

  <footer>
    <p>© 2025</p>
  </footer>
</body>
```

---

## 🔍 Diferença entre tags

- `<article>` → conteúdo independente  
- `<section>` → agrupa conteúdo relacionado  
- `<div>` → sem semântica (uso estrutural/estilização)  

---

## 📈 Próximos passos

- [ ] CSS básico (cores, fontes, box model)
- [ ] Flexbox e Grid
- [ ] Responsividade
- [ ] JavaScript básico
- [ ] Projetos práticos

---

## 💡 Observação

Este repositório faz parte da minha jornada para me tornar desenvolvedora e trabalhar com tecnologia.
