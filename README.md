# Desafio Warren - Web

## Desafio

O desafio será implementar uma tela de lista de transações apresentando os principais dados relacionado a cada uma delas, ao clicar em uma transação será exibido um modal contendo os detalhes desta transação. O desafio deverá conter as seguintes funcionalidades:

- Lista de transações agrupada por data
- Filtro por título
- Filtro por status
- Modal contendo os detalhes da transação

## Telas

Segue abaixo alguns exemplos de telas para uma base, mas sinta-se à vontade para usá-las ou não.

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
- Código (Modularização, Nomenclaturas, Padronização Reutilização);
- Preocupação com usabilidade;

### Interessante (Não fundamental)

- Preocupação com performance;
- Preocupação com acessibilidade;
- TypeScript
- Utilizar alguma lib/framework moderno (React, Vue, Angular, outro)

**Não recomendamos utilizar alguma lib de componentes como, por exemplo, bootstrap, Ant Design, entre outras.**

Mocks utilizados para desenvolver o desafio:

GET: `/api/transactions`

```json
{
  "transactions": [
    {
      "id": 1,
      "title": "Pagamento de boleto",
      "description": "Luz",
      "status": "pending",
      "amount": 100.2,
      "date": "2020-08-12"
    },
    {
      "id": 2,
      "title": "Resgate",
      "description": "Concluí meu objetivo",
      "status": "accepted",
      "amount": 1000,
      "date": "2020-08-12"
    },
    {
      "id": 3,
      "title": "Depósito",
      "description": "Conta",
      "status": "canceled",
      "amount": 5000,
      "date": "2020-08-18"
    },
    {
      "id": 4,
      "title": "Movimentação interna",
      "description": "Férias -> Aposentadoria",
      "status": "pending",
      "amount": 3000,
      "date": "2020-08-12"
    }
  ]
}
```

GET: `/api/transactions/:id`

```json
{
  "title": "Depósito",
  "description": "Aposentadoria",
  "amount": 1000,
  "status": "pending",
  "from": "Banco Chablau",
  "to": "Warren - Portfolio Aposentadoria"
}
```