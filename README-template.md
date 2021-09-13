# Frontend Mentor - FAQ accordion card solution

Essa é a solução para o [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam).

## Sumário

- [Visão Geral](#overview)
  - [O Desafio](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Processo](#my-process)
  - [O Que Aprendi](#what-i-learned)
- [Autor](#author)


## Visão Geral

### O Desafio

Os usuários deverão ser capazes de:

- Ver o layout ideal dependendo do tamanho da tela do dispositivo
- Ver o status hover em todos os elementos com interatividade na página
- Mostrar a resposta quando clicar na pergunta associada

### Screenshot

![desktop](https://user-images.githubusercontent.com/53978097/133126782-710a323d-1d90-4583-a90a-516ea061edbb.png)
![mobile](https://user-images.githubusercontent.com/53978097/133126822-e2190b14-04cd-4c1d-a513-bb510871ed13.png)

### Links

- URL Solução: [Solution URL](https://github.com/Daniel-R23/faq-accordion-card-main)
- URL Site: [Live Site](https://daniel-r23.github.io/faq-accordion-card-main/)

## Processo

### O Que Aprendi

Neste projeto aprendi mais sobre CSS Flex e técnicas de design responsivo. Pude desenvolver a funcionalidade, à priori em JS, com CSS utilizando os seletores, pseudo-classes e pseudo-elementos.

```html
  <div class="acordeao">
    <input type="radio" name="ac" id="ac1">
    <label for="ac1">How many team members can I invite?</label>
    <div class="resposta">
    You can invite up to 2 additional users on the Free plan. There is no limit on
    team members for the Premium plan.</div>
  </div>
```
```css
  label{
      color: var(--cinza-escuro);
    }
    label:hover{
      color: var(--vermelho-claro);
    }
    label:after{
      content: url("images/icon-arrow-down.svg");
      float: right;
    }
    input[name="ac"]{
      display: none;
    }
    .resposta{
      padding-top:10px;
      display: none;
      color: var(--cinza-claro);
      font-size: 0.9em;
    }
    input[name="ac"]:checked~.resposta{
      display: block;
    }
    input[name="ac"]:checked~label{
      font-weight: 700;
    }
    input[name="ac"]:checked~label:after{
      transform: rotateX(180deg);
    }
```

## Autor

- Frontend Mentor - [@Daniel-R23](https://www.frontendmentor.io/profile/Daniel-R23)
