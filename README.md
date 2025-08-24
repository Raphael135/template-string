# 📘 Template Strings em JavaScript (ES6)

## ✨ O que são?

Template Strings (ou Template Literals) são uma forma moderna de criar strings em JavaScript, introduzida no ES6. Elas permitem:

- Criar **strings multilinhas**
- Inserir **variáveis e expressões** diretamente no texto
- Melhorar a **legibilidade** do código

---

## 📌 Sintaxe

Em vez de usar aspas simples `'` ou duplas `"`, usamos **crases** `` ` ``.

```javascript
const nome = "Raphael";
const mensagem = `Olá, ${nome}! Bem-vindo ao mundo do JavaScript.`;
console.log(mensagem); // Olá, Raphael! Bem-vindo ao mundo do JavaScript.
```

---

## 🧠 Interpolação de variáveis

Você pode inserir variáveis ou expressões dentro da string usando `${}`:

```javascript
const a = 5;
const b = 10;
console.log(`A soma de ${a} + ${b} é igual a ${a + b}.`);
// A soma de 5 + 10 é igual a 15.
```

---

## 📄 Strings multilinhas

Com Template Strings, você pode quebrar linhas sem usar `\n`:

```javascript
const texto = `
Essa é uma string
com várias linhas
sem precisar de concatenação.
`;
console.log(texto);
```

---

## 🔍 Comparação com concatenação tradicional

### Antes (modo antigo):

```javascript
const nome = "Raphael";
const idade = 30;
const frase = "Meu nome é " + nome + " e eu tenho " + idade + " anos.";
```

### Agora (com Template String):

```javascript
const nome = "Raphael";
const idade = 30;
const frase = `Meu nome é ${nome} e eu tenho ${idade} anos.`;
```

Muito mais limpo e fácil de ler, né?

---

## ⚠️ Cuidados

- Sempre use **crases** `` ` `` — não funciona com aspas comuns.
- As expressões dentro de `${}` podem ser qualquer código válido: funções, operações, ternários etc.

---

## 🧪 Exemplos avançados

```javascript
const user = { nome: "Raphael", idade: 30 };
const saudacao = `Olá, ${user.nome}. Você tem ${user.idade > 18 ? "maior" : "menor"} de idade.`;
console.log(saudacao);
// Olá, Raphael. Você tem maior de idade.
