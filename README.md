# Projeto-Enigma
Repositório projeto enigma TI. 1B

[Como o programa funciona.md](https://github.com/user-attachments/files/26636145/Como.o.programa.funciona.md)
## **Como o programa funciona?**

A lógica central do código baseia-se no deslocamento fixo do alfabeto. O usuário insere uma mensagem e escolhe um valor de "pulo" (o shift). O programa então percorre cada letra do texto e a substitui pela letra que está algumas posições à frente. Se o deslocamento chegar ao fim do alfabeto (letra Z), o código usa um cálculo matemático (operador de resto % 26) para fazê-lo "dar a volta" e recomeçar pelo A.

O software é dividido em três partes principais:

**-Função de Criptografia:** Soma o deslocamento às letras originais.

**-Função de Descriptografia:** Subtrai o deslocamento para revelar a mensagem real.

**-Preservação:** O código identifica se a letra é maiúscula ou minúscula para não alterar o formato visual da frase e ignora símbolos ou espaços.

## **A Cifra de César e a Enigma**

Diferente da máquina Enigma real, que utilizava rotores complexos que mudavam a substituição a cada letra digitada (criptografia polialfabética), este código utiliza a Cifra de César (substituição monoalfabética). Isso significa que, neste programa, a letra "A" sempre será convertida na mesma letra correspondente durante toda a mensagem, desde que o deslocamento não mude.

## **Limitações do Código**

Apesar de ser um excelente exercício de lógica, este método possui limitações claras de segurança:

**-Vulnerabilidade a Ataques:** Como existem apenas 25 deslocamentos possíveis no alfabeto ocidental, um invasor pode testar todas as combinações (ataque de força bruta) em segundos.

**-Análise de Frequência:** Em textos longos, é fácil descobrir a chave analisando quais letras aparecem mais vezes (como as vogais), já que o padrão de substituição é estático.

**-Simplicidade:** Ao contrário de sistemas modernos ou da própria Enigma, este código não utiliza chaves complexas ou múltiplas camadas de embaralhamento.



