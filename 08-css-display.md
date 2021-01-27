# 08 - Display

Vimos anteriormente que todos os nossos elementos funcionam como uma caixa e que essa caixa tem um certo tamanho \(largura e altura\). Vamos entender agora como essas caixas são posicionadas na tela e como alterar esse posicionamento com a propriedade **display**.

## Block

Algumas **tags** do nosso **HTML** não permitem que outros elementos fiquem lado a lado. Elas ocupam todo o espaço da linha mesmo que o conteúdo não precise desse espaço. A tag **div** é um ótimo exemplo:

```text
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

* * * * >
* * * * * * * * * * * -
* * * * * * * 1. 
* * ```text

  ```
* * * * * 
* 
## Inline

Ao contrário da opção **block** os elementos **inline** ocupam apenas o espaço necessário pelo seu conteúdo permitindo assim que outros elementos ocupem o espaço restante na linha. Vamos ver um exemplo:

```text
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

* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
## Alterando o comportamento padrão:

Podemos facilmente modificar o comportamento padrão de uma **tag** usando a propriedade **display**, vamos voltar ao primeiro exemplo e ver como deixar nossas **div's** ficarem lado a lado como um elemento **inline**:

```text
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

```text
  div {
    display: inline;
  }
```

Com isso a tag **div** irá se comportar como um elemento **inline** deixando os nomes um ao lado do outro.

