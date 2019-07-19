## Flexbox course

### Pre requisites
- html
- css

What is flexbox?
> A: Flexbox is a CSS specification that helps you to design responsive layouts.

#### Material
```shell
wget https://github.com/alura-cursos/posicione-elementos-com-flexbox/archive/809f39a39e473c574e3c6d9d9929626f8d1352fa.zip
```

## Class 01 - the header

#### With CSS
```css
.header {
    display: inline-block;
    vertical-align: middle;
    margin-left: 20px; /* MAGIC NUMBER */
    float: right;
}
```

#### With Flexbox
```css
.class-flex {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```

Which browser can use it ?
> ```shell
> open 'http://caniuse.com'
>```

### display: inline

> Colocando display: inline nos elementos permite eles se posicionarem um do lado do outro, o problema do display: inline é que os elementos não aceitam mais que seja modificada tanto a width quanto a height. Isso limita MUITO nossas possibilidades.

### display: inline-block

>O display: inline-block permite os elementos se posicionarem um do lado do outro porém, diferentemente do display: inline ele permite que os elementos tenham sua width e height modificadas. Por esse motivo o display: inline-block é muito mais interessante na maioria dos casos do que o display: inline.
>
>O problema de usar display: inline-block é espaçar os elementos entre si. Para fazer isso teríamos que colocar margins e fazer contas.

### float: left | right

>O float é mais complicado, ele empurra o elemento para um dos lados (left | right) e os elementos que estão embaixo sobem. Isso nem sempre é o que a gente quer. Além do mais o float não permite que usemos a propriedade vertical-align: middle para alinhar os elementos verticalmente. Ou seja, para contornar isso uma possibilidade seria ter que colocar margin-top ou bottom nos elementos e usar os temidos números mágicos!

### display: flex

>O display: flex veio com o intuito de facilitar nossa vida nesses aspectos de posicionamento. Ele permite os elementos ficarem um do lado do outro, permite espaçar os elementos de forma mais intuitiva e sem ter que fazer cálculos. Além disso ele também permite alinhar os elementos verticalmente de forma fácil.
>
>O display flex pode ser um pouco mais complicado de usar tendo em vista que existem diversas propriedades que vem junto da especificação flexible box, todavia tudo isso foi feito para justamente melhorar nosso código.


---

### Attribute 'justify-content'

The attribute justify content allow you distribute fathers' elements, the possibles values are:
- flex-end : items are packed toward the end line
- flex-start (default): items are packed toward the start line
- center: items are centered along the line
- space-between: items are evenly distributed in the line; first item is on the start line, last item on the end line
- space-around: 
