# Target-Sistemas-Estágio---Ribeirão-Preto

## 1. Sequência de Fibonacci

Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

IMPORTANTE: Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;

```javascript
function pertenceFibonacci(num) {
    if (num < 0) return false;

    let a = 0, b = 1;
    while (b < num) {
        [a, b] = [b, a + b];
    }

    return b === num;
}

const numero = parseInt(prompt("Informe um número para descobrir se ele pertence à sequência Fibonacci:"), 10);
if (pertenceFibonacci(numero)) {
    console.log(`O número ${numero} pertence à sequência de Fibonacci.`);
} else {
    console.log(`O número ${numero} não pertence à sequência de Fibonacci.`);
}
2. Contagem da Letra 'a'
Escreva um programa que verifique, em uma string, a existência da letra ‘a’, seja maiúscula ou minúscula, além de informar a quantidade de vezes em que ela ocorre.

IMPORTANTE: Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;

javascript
Copiar código
function contarLetraA(texto) {
    const textoMinusculo = texto.toLowerCase();
    const contagemA = textoMinusculo.split('a').length - 1;
    
    if (contagemA > 0) {
        console.log(`A letra "A" aparece ${contagemA} vez(es) na string.`);
    } else {
        console.log("A letra \"A\" não aparece na string.");
    }
}

const texto = "Andressa Silva de Aquino";
contarLetraA(texto);
3. Cálculo da Soma
Observe o trecho de código abaixo:

cpp
Copiar código
int INDICE = 12, SOMA = 0, K = 1;
enquanto K < INDICE faça {
    K = K + 1;
    SOMA = SOMA + K;
}
imprimir(SOMA);
Ao final do processamento, qual será o valor da variável SOMA?

O valor da soma será igual a 77.

4. Complete o Próximo Elemento
Descubra a lógica e complete o próximo elemento:

a) 1, 3, 5, 7, 9
b) 2, 4, 8, 16, 32, 64, 128
c) 0, 1, 4, 9, 16, 25, 36, 49
d) 4, 16, 36, 64, 100
e) 1, 1, 2, 3, 5, 8, 13
f) 2, 10, 12, 16, 17, 18, 19, 200

5. Interruptores e Lâmpadas
Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em salas diferentes. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada. Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas?

Na primeira ida, vou verificar apenas uma das lâmpadas. Primeiro, ligarei o interruptor e identificarei qual lâmpada corresponde ao interruptor 1. Depois, retornarei à sala dos interruptores para confirmar qual é o interruptor 1.

Na segunda ida, deixarei uma lâmpada ligada por vários minutos para que ela esquente e, em seguida, desligarei o interruptor para acender outra lâmpada. Ao conferir, a lâmpada que estiver quente e apagada será a que corresponde ao interruptor 2, enquanto a lâmpada que estiver acesa será a que corresponde ao interruptor 3.

