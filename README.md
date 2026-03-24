# estudos-html-css-javascript
Aprendendo o básico do 0

O esqueleto de toda página HTML
Todo arquivo HTML começa com a mesma estrutura base. Pensa como uma casa: tem fundação, paredes e telhado — aqui tem <!DOCTYPE>, <head> e <body>.

O que cada parte faz
Tag/atributo	Para que serve
<!DOCTYPE html>	Ativa o modo HTML5 no navegador. Sem isso, o browser entra em "modo compatibilidade" (mais lento e bugado).
lang="pt-BR"	Diz o idioma da página. Leitores de tela usam isso para pronúncia correta.
charset="UTF-8"	Suporta acentos e caracteres especiais. Sem isso, "ção" vira "��o".
viewport meta	Faz a página funcionar em celular. Sem isso, mobile mostra a versão desktop minúscula.
<title>	Texto que aparece na aba do navegador e no Google.
O que cai em prova
→ Sem charset UTF-8, acentos quebram
→ A meta viewport é obrigatória para responsividade
→ lang no <html> é obrigatório para acessibilidade
→ <head> = configurações invisíveis | <body> = conteúdo visível

HTML semântico vs não-semântico

Errado — div soup
<div class="header">
  <div class="nav">...</div>
</div>
<div class="content">
  <div class="article">
    <div class="title">
      Título
    </div>
  </div>
</div>
<div class="footer">...</div>

Certo — semântico
<header>
  <nav>...</nav>
</header>

<main>
  <article>
    <h1>Título</h1>
  </article>
</main>

<footer>...</footer>

Layout semântico de uma página real

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
      <p>Texto do artigo...</p>
    </article>

    <aside>
      <h3>Relacionados</h3>
    </aside>
  </main>

  <footer>
    <p>© 2025 Meu Site</p>
  </footer>
</body>

Diferença entre article, section e div 
→ <article>: conteúdo independente que faz sentido sozinho (post, notícia, card de produto)
→ <section>: agrupa conteúdos relacionados com um tema. Deve ter um título (h2, h3)
→ <div>: sem significado semântico. Use só para agrupamento visual/CSS, quando nenhuma tag semântica se aplica


