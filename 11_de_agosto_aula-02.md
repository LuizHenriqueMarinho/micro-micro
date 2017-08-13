Quais as diferenças entre os barramentos de dados e de endereços?

Quais são as diferenças entre as memórias RAM e ROM?

Considere o código abaixo:

#include <stdio.h>
int main(void)
{
	int i;
	printf("Insira um número inteiro: ");
	scanf("%d", &i);
	if(i%2)
		printf("%d eh impar.\n");
	else
		printf("%d eh par.\n");
	return 0;
}
Para este código, responda: (a) A variável i é armazenada na memória RAM ou ROM? Por quê? (b) O programa compilado a partir deste código é armazenado na memória RAM ou ROM? Por quê?

Quais são as diferenças, vantagens e desvantagens das arquiteturas Harvard e Von Neumann?

Considere a variável inteira i, armazenando o valor 0x8051ABCD. Se i é armazenada na memória a partir do endereço 0x0200, como ficam este byte e os seguintes, considerando que a memória é: (a) Little-endian; (b) Big-endian.

Sabendo que o processador do MSP430 tem registradores de 16 bits, como ele soma duas variáveis de 32 bits?

Questão 1: o MAB (barramento de endereços na memória) informa endereços e físicos ou locação de memória que o preocessador quer ler ou escrever. A largura de um barramento de dados define a quantidade de memória que ele pode acessar, já o MDB( Barramento de Dados na memóeria) é responsável pelo transporte da instrução ou informação através do código de operação, através de uma variável de processamento ou um sinal de entrada ou saída.
