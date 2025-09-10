alert('Boas vindas ao jogo do número secreto');
let numeroSecreto = parseInt(Math.random() * 100 + 1);
console.log(numeroSecreto);

let chute;
let tentativas = 0; // inicializa

// enquanto chute não for o número secreto continue
while (chute != numeroSecreto) {
    chute = prompt('Escolha um número entre 1 e 100'); // pede de novo o chute
    tentativas++; // conta a tentativa antes de verificar

    if (chute == numeroSecreto) {
        if (tentativas === 1) {
            alert('Isso aí! Você descobriu o número secreto: ' + numeroSecreto +
                  ' em ' + tentativas + ' tentativa!');
        } else {
            alert('Isso aí! Você descobriu o número secreto: ' + numeroSecreto +
                  ' em ' + tentativas + ' tentativas!');
        }
    } else {
        if (chute > numeroSecreto) {
            alert('O número secreto é menor que ' + chute);
        } else {
            alert('O número secreto é maior que ' + chute);
        }
    }
}
