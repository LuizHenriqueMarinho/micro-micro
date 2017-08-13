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

Questão 2: a memória RAM (acesso aleatório) é volátil e perde o cunteúdo quando o sistema é desligado, já a memória ROM (apenas leitura) armazena os dados para qualquer momento, é importante consiliar as duas memórias para um bom sistema embarcado.

Questão 3:
a)para a excecução do código ela é armazenada na memória RAM, a partir do momento que o usuário digitar o valor de i no scanf, o valor passa a ser amarzenado na memória ROM.

b) na memória rom, porém somente a parte que está sendo executata é armazenada na memória RAM, ou seja, por se tratar de um compilador em série, a memória RAM é armazenada linha por linha.

Questão 4: a Havard apresenta os dois sistemas de memória RAM e ROM separados, portanto é mais eficiente e permite uma maior velocidade na excecução, já a arquitetura Von Neumann possúi um sistema único de memória e apesar de ocupar menos espaço acaba tomando muito tempo para processar os dados e o consumo de energia é maior.

Questão 5:
a) little endian 0xDC    0xBA   0x15   0x08
b) big endian 0x80    0x51   0xAB  0xCD

Questão 6: a tranferÊncia acontece com bytes ou palavras de 2 em 2 bits, o seu endereço é dado pelo byte no endereço menor( sempre par) e pode ser lida em um ciclo de clock do barramento.


