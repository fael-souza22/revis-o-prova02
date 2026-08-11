**#-prova02**

**1. O que é o retorno NaN em JavaScript? Cite um tipo de condição em que este tipo pode ser gerado.**

**R:** NaN significa “Not a Number”, ou seja, não é um número. Ele aparece quando o JavaScript não consegue fazer uma operação numérica, como dividir 0 por 0.





**2. É possível adicionar uma configuração CSS de múltiplas formas em um código HTML. Cite essas formas e dê exemplos de cada uma. Cite também a diferença entre utilizar cada uma dessas formas.**

**R:** Existem três formas de usar CSS: inline, interno e externo. O inline é colocado direto na tag, por exemplo: `<p style="color: red;">Texto</p>`. O interno fica dentro da tag `<style>` no HTML. O externo fica em outro arquivo `.css` e é ligado ao HTML. O inline é mais rápido para algo pequeno, o interno pode ser usado em uma página específica e o externo é melhor para organizar e reutilizar os estilos.





**3. Explique a diferença entre as tags `<div>` e `<span>`. Dê exemplos de quando usar cada uma.**

**R:** A `<div>` é usada para organizar partes maiores da página e ocupa uma nova linha. Já a `<span>` é usada em pequenos trechos de texto e não quebra a linha. Por exemplo, podemos usar `<div>` para separar uma seção e `<span>` para mudar a cor de uma palavra.





**4. Descreva o propósito da tag `<head>` em um documento HTML e cite pelo menos três elementos que podem estar dentro dela.**

**R:** A tag `<head>` guarda informações da página que não aparecem diretamente para o usuário. Dentro dela podemos ter `<title>`, `<meta>` e `<link>`. O `<title>` define o nome da aba, o `<meta>` guarda informações da página e o `<link>` pode ligar um arquivo CSS.





**5. Diferencie as listas ordenadas (`<ol>`) das listas não ordenadas (`<ul>`). Crie um exemplo de cada.**

**R:** A lista `<ol>` mostra os itens em ordem, normalmente usando números. A lista `<ul>` usa marcadores e não precisa ter uma ordem.

Exemplo de lista ordenada:

```html
<ol>
  <li>Primeiro</li>
  <li>Segundo</li>
</ol>
```

Exemplo de lista não ordenada:

```html
<ul>
  <li>Arroz</li>
  <li>Feijão</li>
</ul>
```





**6. O que significa a propriedade display no CSS? Compare o comportamento de block, inline e inline-block.**

**R:** A propriedade `display` define como um elemento vai aparecer na página. `block` ocupa uma linha inteira, `inline` ocupa somente o espaço do conteúdo e `inline-block` fica na mesma linha, mas permite definir largura e altura.





**7. Explique o que é o Box Model no CSS e descreva suas partes de dentro para fora.**

**R:** O Box Model mostra como o espaço de um elemento é organizado. De dentro para fora temos: `content` (conteúdo), `padding` (espaço interno), `border` (borda) e `margin` (espaço externo).





**8. Qual é a função das tags semânticas no HTML5, como `<header>`, `<main>`, `<section>` e `<footer>`?**

**R:** As tags semânticas servem para organizar melhor o conteúdo da página. Elas mostram qual é a função de cada parte, como cabeçalho, conteúdo principal, seção e rodapé.




**9. Explique o que é e para que serve o atributo `target="_blank"` em um link. Quais cuidados de segurança devem ser tomados ao utilizá-lo?**

**R:** O `target="_blank"` faz o link abrir em uma nova aba. É recomendado usar junto com `rel="noopener noreferrer"` para evitar problemas de segurança entre as páginas.





**10. O que é a propriedade flex no CSS e como ela é usada?**

**R:** O `flex` é usado para organizar os elementos dentro de um espaço. Ele ajuda a colocar os itens lado a lado e também a controlar o tamanho e o espaço entre eles.





**11. O que são transições (transition) no CSS e como podem ser usadas para criar efeitos de animação simples? Crie um exemplo básico.**

**R:** `transition` serve para fazer uma mudança acontecer de forma suave. Por exemplo, podemos fazer um botão mudar de cor quando o mouse passar por cima.

```css
button {
  background: blue;
  transition: 0.5s;
}

button:hover {
  background: red;
}
```


**12**

const pessoa = {
    nome: "João",
    peso: 70,
    altura: 1.75,
    temperatura: 38.5
};

console.log("Nome:", pessoa.nome);
console.log("Peso:", pessoa.peso, "kg");
console.log("Altura:", pessoa.altura, "m");
console.log("Temperatura:", pessoa.temperatura, "°C");

if (pessoa.temperatura >= 38) {
    console.log("A pessoa está com febre.");
} else {
    console.log("A pessoa não está com febre.");
}

Explicação: o programa cria um objeto pessoa com nome, peso, altura e temperatura. Depois, verifica se a temperatura é igual ou superior a 38 °C.





**13**. Dois objetos do tipo livro
const livro1 = {
    titulo: prompt("Digite o título do primeiro livro:"),
    autor: prompt("Digite o autor do primeiro livro:"),
    ano: Number(prompt("Digite o ano de publicação do primeiro livro:")),
    paginas: Number(prompt("Digite o número de páginas do primeiro livro:")),
    brasileiro: prompt("O autor é brasileiro? (sim/não)").toLowerCase()
};

const livro2 = {
    titulo: prompt("Digite o título do segundo livro:"),
    autor: prompt("Digite o autor do segundo livro:"),
    ano: Number(prompt("Digite o ano de publicação do segundo livro:")),
    paginas: Number(prompt("Digite o número de páginas do segundo livro:")),
    brasileiro: prompt("O autor é brasileiro? (sim/não)").toLowerCase()
};

// Livro com autoria mais antiga
if (livro1.ano < livro2.ano) {
    console.log("Livro com autoria mais antiga:", livro1.titulo);
} else if (livro2.ano < livro1.ano) {
    console.log("Livro com autoria mais antiga:", livro2.titulo);
} else {
    console.log("Os dois livros possuem o mesmo ano de publicação.");
}

// Livro com mais páginas
if (livro1.paginas > livro2.paginas) {
    console.log("Livro com mais páginas:", livro1.titulo);
} else if (livro2.paginas > livro1.paginas) {
    console.log("Livro com mais páginas:", livro2.titulo);
} else {
    console.log("Os dois livros possuem a mesma quantidade de páginas.");
}

// Verificar autor brasileiro
if (livro1.brasileiro === "sim") {
    console.log("Livro com autor brasileiro:", livro1.titulo);
}

if (livro2.brasileiro === "sim") {
    console.log("Livro com autor brasileiro:", livro2.titulo);
}

if (livro1.brasileiro !== "sim" && livro2.brasileiro !== "sim") {
    console.log("Não há livro com autor brasileiro.");
}

Nesse exercício, prompt() permite que o usuário preencha as informações dos dois livros. O programa depois compara o ano, o número de páginas e verifica se algum dos autores é brasileiro.





**14**. Objeto filme e classificação
const filme = {
    nome: prompt("Digite o nome do filme:"),
    classificacao: Number(prompt("Digite a classificação indicativa do filme:"))
};

console.log("Nome do filme:", filme.nome);
console.log("Classificação indicativa:", filme.classificacao, "anos");

if (filme.classificacao === 0) {
    console.log("Faixa etária: Livre");
} else {
    console.log("Faixa etária: Não recomendado para menores de " 
                + filme.classificacao + " anos.");
}

Exemplo de saída:

Nome do filme: Homem-Aranha
Classificação indicativa: 12 anos
Faixa etária: Não recomendado para menores de 12 anos.




**15** Não consegui fazer!




**16. Quais as diferenças entre criar uma variável do tipo const, var e let? Cite exemplos.**

**R:** `var` pode ser redeclarada e tem escopo de função. `let` pode ter seu valor alterado, mas não pode ser redeclarada no mesmo bloco. `const` não pode receber outro valor depois de criada.

Exemplo:

```javascript
var nome = "Ana";
let idade = 20;
const cidade = "São Paulo";
```




**17. Responda no console o que será impresso ou qual erro ocorrerá.**

**R:** O primeiro `x` será `undefined`, porque o `var x` é reconhecido antes de receber o valor. Depois, `x` será 15, `y` será 25 e `z` será 30.

Dentro dos blocos, `a`, `b` e `c` mostram seus valores normalmente. Fora do bloco, `a` continua existindo porque foi criada com `var`, enquanto `b` e `c` não existem fora do bloco. Por isso, `typeof b` e `typeof c` retornam `"undefined"`.

No último bloco, `m` continua existindo fora dele, mas `n` e `o` não. Assim, `typeof m` retorna `"string"` e `typeof n` e `typeof o` retornam `"undefined"`.





**18. Qual a diferença entre JavaScript e Java?**

**R:** Java e JavaScript são linguagens diferentes. Java é muito usado em sistemas e programas maiores e roda na JVM. JavaScript é muito usado em sites para deixar as páginas interativas, mas também pode ser usado no back-end.





**19. Qual a diferença entre `==` e `===` no JavaScript? Dê exemplos práticos.**

**R:** `==` compara os valores e pode converter os tipos. Já `===` compara o valor e também o tipo. Por exemplo:

```javascript
5 == "5"   // true
5 === "5"  // false
```





**20. O que são operadores lógicos (`&&`, `||`, `!`) e como eles podem ser usados em condicionais? Exemplifique.**

**R:** Os operadores lógicos servem para trabalhar com mais de uma condição. `&&` significa “e”, `||` significa “ou” e `!` significa “não”.

Exemplo:

```javascript
if (idade >= 18 && temDocumento) {
  console.log("Pode entrar");
}
```





**21. É possível adicionar novas propriedades a um objeto depois de criado? Como?**

**R:** Sim. Podemos adicionar uma nova propriedade usando ponto ou colchetes.

```javascript
let pessoa = {
  nome: "Lucas"
};

pessoa.idade = 22;
```

Também podemos fazer:

```javascript
pessoa["cidade"] = "São Paulo";
```





**22. Qual a diferença entre null e undefined no JavaScript?**

**R:** `null` significa que o valor foi colocado como vazio de propósito. `undefined` significa que a variável ainda não recebeu um valor.

Exemplo:

```javascript
let x = null;
let y;
```

Nesse caso, `x` é `null` e `y` é `undefined`.





**23. O que é um objeto em JavaScript e como ele é declarado? Dê um exemplo básico.**

**R:** Um objeto serve para guardar várias informações relacionadas. Ele é criado usando `{}`.

```javascript
let pessoa = {
  nome: "Lucas",
  idade: 22,
  cidade: "São Paulo"
};
```

Nesse exemplo, `pessoa` tem as informações de nome, idade e cidade.
