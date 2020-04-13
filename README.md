# CSS Grid e Flexbox - Quando utlizar?

Construindo layouts comuns com CSS Grid e Flexbox.

Alguns layouts utilizados:

- Globo .com
- Youtube

---

## Grid layout sample

Curso pago Origamid: https://www.youtube.com/redirect?v=x-4z_u8LcGc&event=video_description&q=https%3A%2F%2Fwww.origamid.com%2Fcurso%2Fcss-grid-layout&redir_token=rBsimRNIxZwsvHgKC0D2jkVkFop8MTU4NjcyODcxNUAxNTg2NjQyMzE1

### Base
```
.gridClass {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* 2 colunas com 1 fração cada */
    grid-grap: 20px; /* Funciona como se aplicasse margem entre os itens */
    margin: 0 auto; /* Centraliza itens na tela */
    max-width: 800px; /**/
    padding: 10px;
}
```

### Definindo altura de determinado item na tela

```
.gridItem:nth-child(1) {
    grid-row: 1 / 3; /* Vai ocupar da linha 1 até a 3 */
}
```
---
## Flexbox layout sample

Curso gratuito Origamid: https://www.origamid.com/curso/css-flexbox/2-1-display-flex
```
.flexboxClass {
    display: flex;
    flex-wrap: wrap;
    max-width: 800px;
    margin: 0 auto;
}

.flexboxClass>div {
    flex: 1 1 200px;
    margin: 10px;
}
```

## Devo utilizar float, grid layout ou flexbox?

Depende do público alvo da aplicação

Em 2020, 89,78% dos browsers aceitam grid layout. Porem, se esses 11% restantes significam um número relevante ou se são justamente meu público alvo, não deve-se utlizar grid layout ou flexbox.

- Browsers antigos não suportam grid layout ou flexbox, então deve-se utlizar float quando necessário.

Apesar de tudo, atualmente são as melhores opções disponíveis.
