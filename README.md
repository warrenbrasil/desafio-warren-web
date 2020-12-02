# Desafio Warren - Web

## Desafio

O desafio será implementar uma tela de lista de transações apresentando os principais dados relacionado a cada uma delas, ao clicar em uma transação será exibido um modal contendo os detalhes desta transação. O desafio deverá conter as seguintes funcionalidades:

- Lista de transações agrupada por data
- Filtro por título
- Filtro por status
- Modal contendo os detalhes da transação

## Telas

Segue abaixo alguns exemplos de telas para uma base, mas sinta-se à vontade para usá-las como referência ou não.

### Lista de transações

![https://lh4.googleusercontent.com/Ga-DeKt5_ZGnwh7YsPrn0QCJbkGV-RdbSFglK-xNPyFScZ1OkWqYJB7lm2r2Ht5i_tKC35-RQw0u6XMm_FCd5-qv9eBLKoR2OZ6WSwi4daDsTdzQk73Doyt-FlS65C6pHA_UUxxo](https://lh4.googleusercontent.com/Ga-DeKt5_ZGnwh7YsPrn0QCJbkGV-RdbSFglK-xNPyFScZ1OkWqYJB7lm2r2Ht5i_tKC35-RQw0u6XMm_FCd5-qv9eBLKoR2OZ6WSwi4daDsTdzQk73Doyt-FlS65C6pHA_UUxxo)

### Modais

#### Modal de depósito
![https://lh3.googleusercontent.com/U-NHHZ9enUvNbT7Kvx2cmCzr9yzpXi1GVGY007d2wJ20IrE-p7xxRuOCxa8yyBwWiK_rcPjHhiLvKK5C_jnNLXlMptNW3DCTe41GAuyEkguh3WOLnvVkcvBUBLL9HZTxiQH5UwGV](https://lh3.googleusercontent.com/U-NHHZ9enUvNbT7Kvx2cmCzr9yzpXi1GVGY007d2wJ20IrE-p7xxRuOCxa8yyBwWiK_rcPjHhiLvKK5C_jnNLXlMptNW3DCTe41GAuyEkguh3WOLnvVkcvBUBLL9HZTxiQH5UwGV)


#### Modal de resgate
![https://lh3.googleusercontent.com/4HjLEYZxJl8tMZvjfeMI5SGoIY--Us9aXHMxw8R9So-qH1imMbCGwORsXVqZ2D95n2nXiN9JaEYFHa61mAI8M2R0hEUdPZubVShE1qBpVHgPgF-4XAzZJG4aBaFb1w5xIsuzRN6l](https://lh3.googleusercontent.com/4HjLEYZxJl8tMZvjfeMI5SGoIY--Us9aXHMxw8R9So-qH1imMbCGwORsXVqZ2D95n2nXiN9JaEYFHa61mAI8M2R0hEUdPZubVShE1qBpVHgPgF-4XAzZJG4aBaFb1w5xIsuzRN6l)


#### Modal de Movimentação interna
![https://lh6.googleusercontent.com/fN6UH8MXdeSPGj6NfHmZwbqOshOf5bOqVDrboCJD2gyXyZBFCT_duBPe6V0gc06rTi_LE1wtV5tH7ziogCfvPQsofcsUhRWqcwKC4poQiybwsPMGUmhql315-A4LHRsu-iuKgbBU](https://lh6.googleusercontent.com/fN6UH8MXdeSPGj6NfHmZwbqOshOf5bOqVDrboCJD2gyXyZBFCT_duBPe6V0gc06rTi_LE1wtV5tH7ziogCfvPQsofcsUhRWqcwKC4poQiybwsPMGUmhql315-A4LHRsu-iuKgbBU)

## Tecnologias

Aqui na Warren utilizamos as seguintes tecnologias, novamente sinta-se à vontade para usá-las ou não.

- VueJs
- TypeScript
- Webpack
- Less
- Jest
- Cypress
- Axios

## O que será avaliado

### Principal

- Documentação (comente sobre decisões técnicas, escolhas, requisitos, etc);
- Testes (muito importante!);
- Design da solução/arquitetura;
- Código (Modularização, Nomenclaturas, Padronização, Reutilização);
- Preocupação com usabilidade;
- Utilizar alguma lib/framework moderno (React, Vue, Angular, outro)

### Interessante (Não fundamental)

- Preocupação com performance;
- Preocupação com acessibilidade;
- TypeScript

**Não recomendamos utilizar alguma lib de componentes como, por exemplo, bootstrap, Ant Design, entre outras.**

Mocks utilizados para desenvolver o desafio:

GET: `https://warren-transactions-api.herokuapp.com/api/transactions`

```json
[
  {
    "id": "5f89f9f257fe42957bf6dbfd",
    "title": "Resgate",
    "description": "et labore proident aute nulla",
    "status": "created",
    "amount": 2078.66,
    "date": "2018-12-22",
    "from": "Aposentadoria",
    "to": "Conta Warren"
  },
  {
    "id": "5f89f9f271e4213092bd4e41",
    "title": "Depósito",
    "description": "excepteur veniam proident irure pariatur",
    "status": "created",
    "amount": 148856.29,
    "date": "2017-07-23",
    "from": "Trade",
    "to": "Conta Warren"
  },
  {
    "id": "5f89f9f2f318e70ff298f528",
    "title": "Movimentação interna",
    "description": "eu officia laborum labore aute",
    "status": "processed",
    "amount": 25092.8,
    "date": "2016-08-25",
    "from": "Férias",
    "to": "Trade"
  },
  {
    "id": "5f89f9f235a90e5336c796f7",
    "title": "Movimentação interna",
    "description": "labore id culpa magna minim",
    "status": "created",
    "amount": 172513.46,
    "date": "2020-04-29",
    "from": "Férias",
    "to": "Conta Warren"
  },
  {
    "id": "5f89f9f23e427f64fc2ea101",
    "title": "Depósito",
    "description": "aute aliqua eu excepteur et",
    "status": "processing",
    "amount": 51668.85,
    "date": "2020-01-01",
    "from": "Férias",
    "to": "Conta Warren"
  }
]
```

GET: `https://warren-transactions-api.herokuapp.com/api/transactions/:id`

```json
{
  "id": "5f89f9f23e427f64fc2ea101",
  "title": "Depósito",
  "description": "aute aliqua eu excepteur et",
  "status": "processing",
  "amount": 51668.85,
  "date": "2020-01-01",
  "from": "Férias",
  "to": "Conta Warren"
}
```
