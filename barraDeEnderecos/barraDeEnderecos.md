# Funções
Primeiramente para entender o conceito do link no javascript
precisamos primeiro aprender o que é uma função.
Uma função é basicamente uma parte separada do código que processa uma determinada informação e pode ser invocada a qualquer momento do código. 

Uma função normalmente é utilizada para melhorar o entendimento do código e trazer mais clareza. Separando partes do código fica mais fácil de entender o que cada parte faz. Como podemos chamar essa parte do código a qualquer momento as funções também contribuem para a reutilização do código. 

Para exemplificar melhor esse conceito utilizaremos paralelos matemáticos. 
Vamos supor que eu queira fazer um programa que diga se um aluno foi aprovado ou não em um ano letivo e a média mínima para passar de ano é 7. Mas eu quero criar uma função que calcule apenas a média do aluno.

```
/* Função criada para calcular a média  */
function media(nota1, nota2, nota3, nota4){
	var mediaCalculada = (nota1 + nota2 + nota3 + nota4)/4
	return mediaCalculada; 
} 
/* código principal(main) */
/* declaração de variáveis*/
var nota1 = 5, 
	nota2 = 6,
	nota3 = 7,
	nota4 = 8;

/* chamando a função média e passando as notas como argumentos. Resultado recebe o valor da média das 4 notas */
var resultado = media(nota1,nota2,nota3,nota4); 

/* utilizando a variável resultado que recebeu a */
if(resultado >= 7){
	console.log("Parabéns! Você foi aprovado");
}else{
	console.log("você foi reprovado");
}
		
``` 

# Links em HTML 

Outro conceito importante para entender a chamada do javascript através de links é o conceito de links em HTML. 
Quando queremos passar o endereço de uma página em html uzamos a *tag* `<a>`. 
A sintaxe da *tag* é `<a href="url">link text</a>`
desse jeito quando clicarmos nas palavras *link text* seremos redirecionados para o site que definimos através do campo *href*. 
Um exemplo Real seria: 

``` <a href="https://www.google.com/">link Para o google</a> ``` 
- <a: indicador da *tag* de hiperlink. 
- href: atributo que referencia o endereço do site, nesse caso o google. O atributo href também pode referenciar uma função javascript.
- link Para o Google: Texto que redireciona para o site do google. 
- `</a>` : Fechamento da *tag* indicando que o texto do link acabou.

# Utilizando href na chamada do link em javascript 

Utilizando javascript nós podemos deixar página de web dinâmicas. Ou seja, alterar a página durante o uso. É possível chamar uma função javascript em um elemento html através da *tag* `<a>` e assim permitir que um elemento html esteja associado a algum evento ou alguma modificação no javascript. 

Para exemplicar essa situação de associar uma função à seleção de um link temos o código abaixo. Neste caso ela será chamada quando o ocorrer o evento de clique no link.
Vemos que esse código abre uma janela escrita "Você clicou" quando clicamos no texto "Clique aqui"

Para que o procedimento funcione, é necessário incluir a string 'javascript:' na chamada da função, dentro do atributo *href* da *tag* a do html. Como o padrão do atributo href é uma url é importante sinalizar que é uma função javascript para não haver riscos de interpretação errada.

Exemplo:

```
/* código javascript */
<script>
/*construção da função clicou*/
function clicou(){
window.alert("Parabéns! Você clicou");
}
/*encerramento do javascript */
</script>
```

A chamada no código HTML:

```
<a href="javascript:clicou()">Clique aqui</a>
```
Nesse caso quando o texto *Clique aqui* for clicado vai aparecer uma janela escrito "Parabéns! Você clicou". 