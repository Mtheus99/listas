#lista de prog. Lucas Int.


//5)

#include <stdio.h>

int main(void) {
  int x,i;
  printf("insira um numero entre 1 a 5\n");
  scanf("%i",&x);
  switch(x){
    case 1:
     printf("numero ordinal: %dº",x);
     printf(" (Primeiro)");break;
    case 2:
     printf("numero ordinal: %dº",x);
     printf(" (Segundo)");break;
    case 3:
     printf("numero ordinal: %dº",x);
     printf(" (Terceiro)");break;
    case 4:
     printf("numero ordinal: %dº",x);
     printf(" (Quarto)");break;
    case 5:
     printf("numero ordinal: %dº",x);
     printf(" (Quinto)");break;
  }
 
  return 0;
}
------------------------------------------------------------------------
#include <stdio.h>
#include <stdlib.h>

//4)
int main()
{   int x;
    float b,h,ld,c,lar,r;
    float C,T,Q,R;
    printf("Qual figura deseja calcular a area?\n\n");
    printf("1. Circulo\n2. Triangulo\n3. Quadrado\n4. Retangulo\n\n");
    scanf("%d",x);
    switch(x){
    case 1:
        printf("Informe o raio da circunferencia:\n");
        scanf("%f",&r);
        C = 3.14*(r*r);
        printf("A area do circulo e: %g",C);
    case 2:
        printf("Informe a Base e Altura do triangulo:\n");
        scanf("%f%f",&b,&h);
        T = (b*h)/2;
        printf("A area do triangulo e: %g\n",T);
    case 3:
        printf("Informe um lado do quadrado:\n");
        scanf("%f",ld);
        Q = ld*ld;
        printf("A area do quadrado e: %g\n",Q);
    case 4:
        printf("Informe o comprimento e altura do retangulo:\n");
        scanf("%f%f",&c,&lar);
        if(c>lar||c<lar){
            R = c*lar;
            printf("A area do retangulo e: %g\n",R);
        }else
            printf("Os lados informados correspondem a um quadrado:)");
            R = c*lar;
            printf("A area do quadrado e: %g\n",R);
    }


    return 0;
}
--------------------------------------------------------------------------------

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
//3)
int main()
{   float a,b,c,delta,x1,x2;
    printf("Informe os coeficientes da equaçao(a,b,c): \n");
    scanf("%f%f%f",&a,&b,&c);
    delta = (b*b) - (4*(a*c));
    if(delta!= 0){
        if(delta>0){
        x1 = ((b*(-1))+ sqrt(delta))/2*a;
        x2 = ((b*(-1))- sqrt(delta))/2*a;
        printf("\nAs raizes da equaçao sao: %g e %g",x1,x2);
    }else printf("Nao existe raiz real. \n");

    }else {
        x1 = (b*(-1))/2*a;
        x2 = x1*(-1);
        printf("\nAs raizes da equaçao sao: %g e %g",x1,x2);
    }

    return 0;
}
------------------------------------------------------------------------------

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
//2)
int main()
{   float ps,pd;
    printf("Informe as pressoes sistolica e diastolica da pessoa: \n");
    scanf("%f%f",&ps,&pd);
    if(ps<=120&&pd<=80){
        printf("\nPressao arterial ideal! \n");
        printf("\nCandidato apto para o experimento!\n ");
    }else
        printf("\nCandidato inapto para o experimento!\n ");
    return 0;
}

