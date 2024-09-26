1. Encadiando seletores

h1, .time {
    background-color: red;
}

2. Usando a pseudoclasse is que permite selecionar varios seletores de uma só vez

:is(h1, .time) {
    background-color: red;
}

