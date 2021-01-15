## Display

Vimos anteriormente que todos os nossos elementos funcionam como uma caixa e que essa caixa tem um certo tamanho (largura e altura). Vamos entender agora como essas caixas são posicionadas na tela e como alterar esse posicionamento com a propriedade **display**.

### Block

Algumas **tags** do nosso **HTML** não permitem que outros elementos fiquem lado a lado. Elas ocupam todo o espaço da linha mesmo que o conteúdo não precise desse espaço. A tag **div** é um ótimo exemplo:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
  <div>
    Kelvin
  </div>
  <div>
    Kraken
  </div>
</body>
</html>
```

No exemplo acima os nomes serão renderizados um acima do outro, isso acontece porque o comportamento padrão da **div** é **block**. Isso significa que a **tag** irá ocupar todo o espaço da linha não permitindo que outros elementos fiquem ao seu lado.

Essas são as tags que tem o comportamento **block**:

- <address>
- <article>
- <aside>
- <blockquote>
- <canvas>
- <dd>
- <div>
- <dl>
- <dt>
- <fieldset>
- <figcaption>
- <figure>
- <footer>
- <form>
- <h1>-<h6>
- <header>
- <hr>
- <li>
- <main>
- <nav>
- <noscript>
- <ol>
- <p>
- <pre>
- <section>
- <table>
- <tfoot>
- <ul>
- <video>

### Inline

Ao contrário da opção **block** os elementos **inline** ocupam apenas o espaço necessário pelo seu conteúdo permitindo assim que outros elementos ocupem o espaço restante na linha. Vamos ver um exemplo:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
  <span>
    Kelvin
  </span>
  <span>
    Kraken
  </span>
</body>
</html>
```

A tag **span** tem por padrão o comportamento **inline**, isso significa que a tag irá ocupar apenas o espaço necessário para o texto fazendo com que os nomes sejam renderizados lado a lado.

Essas são as tags que tem o comportamento **inline**:

- <a>
- <abbr>
- <acronym>
- <b>
- <bdo>
- <big>
- <br>
- <button>
- <cite>
- <code>
- <dfn>
- <em>
- <i>
- <img>
- <input>
- <kbd>
- <label>
- <map>
- <object>
- <output>
- <q>
- <samp>
- <script>
- <select>
- <small>
- <span>
- <strong>
- <sub>
- <sup>
- <textarea>
- <time>
- <tt>
- <var>

### Alterando o comportamento padrão:

Podemos facilmente modificar o comportamento padrão de uma **tag** usando a propriedade **display**, vamos voltar ao primeiro exemplo e ver como deixar nossas **div's** ficarem lado a lado como um elemento **inline**:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
  <div>
    Kelvin
  </div>
  <div>
    Kraken
  </div>
</body>
</html>
```

Vamos sobrescrever o comportamento da nossa tag **div** usando o **display**:

```
  div {
    display: inline;
  }
```

Com isso a tag **div** irá se comportar como um elemento **inline** deixando os nomes um ao lado do outro.