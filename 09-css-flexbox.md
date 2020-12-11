## Flexbox

O flexbox é a primeira tecnologia do **css** pensada para os layouts da
web moderna, diferente das técnicas antigas (float, inline-block, position)
ele traz a felxibilidade e a robustez necessária para se criar layouts complexos com mais facilidade.

### Ativando o flexbox!

Para ativar o flexbox em algum elemento na página nós usamos a propriedade display:

```
.container {
  display: flex;
}
```

A partir desse momento todos os filhos dessa classe irão se comportar como **flex items** (falaremos sobre eles abaixo).

### Entendendo os eixos!

Após a ativação do **flexbox** nós podemos configurar algumas opções no nosso container como o alinhamento horizontal e vertical, o flexbox funciona baseado em **eixos**: **eixo principal** e **eixo secundário**.


### Eixo principal!

Para modificarmos o alinhamento dos items dentro do eixo principal nós usamos a propriedade **justify-content**, nós temos as seguintes opções:

* **flex-start**
* **flex-end**
* **center**
* **space-around**
* **space-between**
* **space-evenly**

![flexbox - main axis](https://raw.githubusercontent.com/VaiNaWeb/gitbook-assets/master/modulo-1/images/flexbox-main-axis.png)

### Eixo secundário!

Para modificarmos o alinhamento dos items dentro do eixo secundário nós usamos a propriedade **align-items**, nós temos as seguintes opções:

* **flex-start**
* **flex-end**
* **center**
* **stretch**
* **baseline**

![flexbox - cross axis](https://raw.githubusercontent.com/VaiNaWeb/gitbook-assets/master/modulo-1/images/flexbox-cross-axis.png)