# calculo-em-C


   #include <stdio.h>
  
 int main(){
       float num1, num2, resultado;
       char operador;

           printf("digite uma operação (+,-,*,/)");
           scanf("%c",&operador);
           printf("digite o primeiro numero: ");
           scanf("%f",&num1);
           printf("digite o segundo numero:");
           scanf("%f",&num2);
         
        switch (operador){
               case '+':
                    resultado= num1+num2;
                    printf("resultado: %.2f\n", resultado);
                    break;
               case '-':
                    resultado= num1-num2;
                    printf("resultado: %.2f\n", resultado);
                    break;
               case '*':
                    resultado= num1*num2;
                    printf("resultado: %.2f\n", resultado);
                    break;
               case '/':
                  if(num2!=0){
                        resultado= num1/num2;
                           printf("resultado: %.2f\n", resultado);
                  }
                   else 
                        printf("erro: divisão por zero!\n");
                          break;
                    default:
                        printf("operador invalido\n");
        }
      return 0;
 }
 
