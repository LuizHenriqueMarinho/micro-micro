Para todas as questões, considere que as variáveis f, g, h, i e j são do tipo inteiro (16 bits na arquitetura do MSP430), e que o vetor A[]
é do tipo inteiro. Estas variáveis estão armazenadas nos seguintes registradores:

f: R4
g: R5
h: R6
i: R7
j: R8
A: R9
Utilize os registradores R11, R12, R13, R14 e R15 para armazenar valores temporários.

Traduza as seguintes linhas em C para a linguagem assembly do MSP430. Utilize somente as seguintes instruções: mov.w, add.w, 
sub.w, clr.w, dec.w, decd.w, inc.w e incd.w.
(a) f *= 5;
add.w   R4,R4  // mujltiplicar nada mais é que somar.
add.w   R4,R4   
add.w   R4,R4   
add.w   R4,R4   


(b) g *= 6;
o mesmo da questão 5 com mais uma linha.

(d) A[2] = 6*A[1] + 5*A[0];
add.w 1(R9),1(R9)   //2*1(R9)
add.w 1(R9),1(R9)   //3*1(R9) 
add.w 1(R9),1(R9)   //4*1(R9) 
add.w 1(R9),1(R9)   //5*1(R9) 
add.w 1(R9),1(R9)   //6*1(R9) 
add.w 0(R9),0(R9)   //2*0(R9) 
add.w 0(R9),0(R9)   //3*0(R9) 
add.w 0(R9),0(R9)   //4*0(R9) 
add.w 0(R9),0(R9)   //5*0(R9)
add.w 0(R9),1(R9)   // 6*1(R9) = 5*0(R9) + 6*1(R9)
mov.w 1(R9),2(R9)   // 2(R9) = 6*1(R9) = 5*0(R9) + 6*1(R9)


(e) A[3] = 3*f - 5*h;


(f) A[5] = 6*(f - 2*h);
