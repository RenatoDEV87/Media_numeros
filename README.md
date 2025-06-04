# Fazer um algoritmo para receber números decimais até que o usuário digite 0 e fazer amédiaaritmética desses números

# Exercício 13: Média Aritmética de Números Decimais

---

## 📑 Índice

1. [📖 Descrição](#descrição)  
2. [💻 Código](#código)  
3. [🚀 Como Executar](#como-executar)   
4. [🛠️ Tecnologias Utilizadas](#tecnologias-utilizadas)  
5. [📜 Licença](#licença)  

---

## Descrição

Este programa em JavaScript recebe números decimais do usuário até que ele digite 0. Após isso, calcula e exibe a média aritmética dos números digitados (excluindo o zero).

---

## Código

Abaixo está o código-fonte do programa:

```JavaScript
// Este programa calcula a média aritmética de números decimais inseridos pelo usuário até ele digitar 0

const prompt = require('prompt-sync')();

let soma = 0;
let quantidade = 0;
let numero;

do {
  numero = parseFloat(prompt("Digite um número decimal (ou 0 para sair): "));
  
  if (numero !== 0) {
    soma += numero;
    quantidade++;
  }

} while (numero !== 0);

if (quantidade > 0) {
  let media = soma / quantidade;
  console.log(`\nA média dos números digitados é: ${media.toFixed(2)}`);
} else {
  console.log("Nenhum número válido foi digitado.");
}

```

---

## Como Executar

🛠️ Instruções para executar localmente

1. Instale o Node.js se ainda não tiver: https://nodejs.org

2. Abra o terminal e instale o prompt-sync (usado para entrada do usuário):

```
npm install prompt-sync
```

3. Salve o arquivo como `exercício_13.js` e execute com:

```
node exercício_13.js
```

---

## Tecnologias Utilizadas

- Linguagem: JavaScript
- Node.Js

---

## Licença

Este projeto está licenciado sob a MIT License.
