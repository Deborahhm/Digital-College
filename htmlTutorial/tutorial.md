# Tags
![tag HTML](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/tag.drawio.png)

O html é uma linguagem de marcação de texto. E essas marcações são feitas através de tags. A tag tem uma estrutura em que o elemento ( nesse caso o p) fica dentro de dois sinais. É através das tags que indicamos o que acontece ou o que é o texto. 
Por exemplo:  quando eu escrevo um páragrafo eu posso escrever em html 
`<p> Isso é um parágrafo </p>` . 
Veja que o texto fica entre as tags de abertura e fechamento. Isso porque precisamos indicar ao navegador que o parágrafo acabou. O elemento "p" indica que o texto dentro daquelas tags é um parágrafo. todo elemento possuí uma função específica no HTML. "p" é paragrafo, "a" é link, "img" é imagem e teremos muitos outros outros.
No entanto nem todos os elementos possuem tags de fechamento. 

## Self-closing tags e atributos
Como foi falado anteriormente nem todas as tags possuem tag de fechamento. Um exemplo disso é tag img. Que não possue tag de fechamento 
`<img src="img_url.png" alt="legenda da imagem">` . Vemos que o endereço da imagem está na verdade dentro da tag e é passado como o valor de um atributo. 

![atributo da tag](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/atribute.drawio.png)

Os atributos adicionam informações adicionais para as tags. No caso do parágrafo da imagem temos o atributo *lang*, que especifica que a linguagem do parágrafo é inglês.  Já no caso da imagem temos os atributo *src* que contém a *url* ou caminho da imagem e o atributo *alt*  que contém a legenda da imagem. No geral, a estrutura da tag pode ser escrita assim: 
![Estrutura da tag](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/tagstructure.drawio.png)

# Estrutura de um documento html

As tags do html também são estruturais e seguem uma certa hierarquia para o texto ser organizado e padronizado. 
## Body
Temos abaixo uma estrutura simplificada de um documento html. Podemos verificar de uma maneira mais visual a abertura e fechamento das tags.
![estruturahtml](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/htmlstructure.drawio.png)
- `<html>` :  tag de abertura de um documento html propriamente dito, todas as tags deverão ficar dentro dessa tag ]. É ela quem marca onde começa e onde termina um documento html. 
- `<body>`: O corpo do html, é nessa tag que deve ficar o contéudo principal e toda a parte visual do site.
- `<h1>,<h1>`: Cabeçalhos utilizados para indicar títulos em documentos. Diferenciados apenas pelos tamanhos de suas fontes. 
- `<p>`: Como já falamos anteriormente o p é utilizado para marcar um parágrafo. 

É sempre importante identar bem as tags e tentar pensar nelas comos blocos que englobam outras tags ou tags englobadas por esses blocos, nesse caso a tag `<hmtl>` é um bloco que contém todas as outras tags, é a tag que indica onde o documento começa e onde ele termina. 

## Head
Como falei antes, esse exemplo é uma estrutura simplificada e apesar de funcionar em um navegador não é a mais adequada porque é importante que exista a tag head. Podemos ver abaixo uma estrutura completa de html.

![Estrutura completa HTML](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/htmlstructure2.drawio.png)

Podemos ver que acima da tag *body* temos a tag *head*. É na tag head que fica informações como o título da página e é onde normalmente colocamos o link para documentos de css e scripts. Vemos abaixo o equivalente html da página 

```
<!DOCTYPE html>
<html>
	<head>
		<link rel="stylesheet" href="styles.css">
		<title>Isso é um titulo</title>
	</head>
	<body>
		<h1>Isso é um cabeçalho</h1>
		<p> Esse texto é um páragrafo e assim como na língua portuguesa serve para escrever um texto sobre algo </p>
		<h2>Isso é um sub-cabeçalho</h2>
		<p> Vários artigos possuem sub-cabeçalhos para te ajudar a seguir uma estrutura mais organizada de texto. Divindo em pequenas partes. </p>
		<h2> Outro sub-cabeçalho </h2>
		<p> Aqui em cima você pode ver outro sub-cabeçalho </p>
	</body>
</html>
```

![estrutura html no navegador](https://raw.githubusercontent.com/Deborahhm/Digital-College/main/htmlTutorial/images/htmlestrutura.png)

## Meta tags 
Normalmente o elemento head contém informações que não aparecem visualmente na página, exceto o título. Mas essas informações são importantes para o correto funcionamento da página e para os buscadores de site. Normalmente esse tipo de informação está presente em meta tags 

```
<head>
  <meta charset="UTF-8"> < !--Especifica a codificação de caracteres -- >
  <meta name="description" content="Free Web tutorials"> 
  < !--Descrição do documento -- >
  <meta name="keywords" content="HTML, CSS, JavaScript">
   < !-- Palavras chaves do documento -- >
  <meta name="author" content="John Doe">
   < !-- Autor -- >
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  < !-- Informaçoes sobre a visualização da tela -- >
</head>
```

## Comentários 

Um comentário html segue o formato `< !-- Isso é um comentário -- >` 
O comentário não aparece no navegador e também não tem nenhuma informação que o código precise para funcionar. Mas é utilizado para organizar o código e explicar para outras pessoas o que está acontecendo no seu código.

# Imagens e links 

Duas tags muito importantes para a construção de sites são as tags de imagens e links, vamos aprender um pouco mais sobre elas 
## Elemento `<a>`

O elemento "a"
## Elemento `<img>`
## Elemento `<figure>`

# Listas 

