Um atributo é tudo vinculado a uma tag

h1[title] {
    background-color: red;
}

entao eu to aplicando em toda h1 que possui um title como atributo

1. Posso selecionar o atributo de forma isolada
[Title] {
    background-color: red;
}


2. Selecionar um valor do atributo
[title="titple1] {
    background-color: red;
}

3. Selecionando diretamente o id
[id="rating"] {
    background-color: green;
}

4. Consigo concatenar atributos dessa forma
[id="comments-list"] > [data-user="João"] {
    background-color: pink;
}
aqui eu seleciono um filho direto do atributo inicial "comments-list"

[class="categories"] {
    background-color: red;
}

[data-recipe~="de"] {
    background-color: lightblue;
}

podemos selecionar uma palavra como vemos a cima, nesse caso selecionamos apenas as linhas
que possuem a palava "de" seguida e antecipada de um espaço




podemos também concatenar com virgula
o ~= é um identificador de uma palavra que pertence ao atributo
[data-recipe~="de"],
[data-tipe~="bolo"] {
    background-color: red;
}

4. Selecionando um elemento que tem uma palavra especifica em sequencia
no caso ele irá selecionar todo o atributo style que é seguito de uma
palavra "font" seguida de um hífen

[style|="font"] {
    background-color: violet;
}

5. Podemos selecionar uma classe ou id que é iniciado por um prefixo especifico(prefixo)
[class^="r"], 
[data-question^="Posso"] {
    background-color: orange;
}

6. Agora vamos selecionar uma classe que possui um (sufixo) especifico
[class$="es"] {
    background-color: purple;
}

7. Agora vamos selecionar uma classe que possui um conjunto no meio dela, ou qualquer ocorrencia 
sendo no começo, meio ou fim
[class*="ommen"] {
    background-color: bisque;
}

8. Se quisermos ignorar a ocorrencia de letras maiusculas ou minusculas usamos o "i" ou "I"
[data-user*="A" I] {
    background-color: bisque;
}