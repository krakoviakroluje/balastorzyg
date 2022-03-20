# balastorzyg
# #include <stdio.h>
#include <stdlib.h>
#include <math.h>
int main()
{
    //wzór: y = a0x0+a1x1+a2x2+a3x3+a4x4+a5x5+a6x6+a7x7+a8x8
    //współczynniki
    float a0, a1, a2, a3, a4, a5, a6, a7, a8;
    //zmienne
    float x,y;
    //stała odległość
    float dx;
    //pole
    float area = 0;
    //x początkowy x końcowy
    int xp, xk;
    //potęga wielomianu
    int potega;

    printf("Enter xp and xk: \n");
    scanf("%d %d", &xp, &xk);
    printf("Enter dx: ");
    scanf("%f", &dx);
    printf("Wpisz potege: ");
    scanf("%d", &potega);
    //fail
    /*for(x = xp; x<= xk; x = x+dx)
    {
        switch(potega)
        {
        case 0:
            printf("Podaj a0: ");
            scanf("%f", a0);
            y = a0*pow(x, 0);
            area = area + y*dx;
        printf("x:%f y:%f Area:%f\n",x ,y, area);



        case 1:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            y = a0*pow(x, 0) + a1*pow(x, 1);



        case 2:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2);



        case 3:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3);



        case 4:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            printf("Podaj a4: ");
            scanf("%f", a4);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4);



        case 5:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            printf("Podaj a4: ");
            scanf("%f", a4);
            printf("Podaj a5: ");
            scanf("%f", a5);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5);



        case 6:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            printf("Podaj a4: ");
            scanf("%f", a4);
            printf("Podaj a5: ");
            scanf("%f", a5);
            printf("Podaj a6: ");
            scanf("%f", a6);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6);




        case 7:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            printf("Podaj a4: ");
            scanf("%f", a4);
            printf("Podaj a5: ");
            scanf("%f", a5);
            printf("Podaj a6: ");
            scanf("%f", a6);
            printf("Podaj a7: ");
            scanf("%f", a7);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6) + a7*pow(x, 7);




        case 8:
            printf("Podaj a0: ");
            scanf("%f", a0);
            printf("Podaj a1: ");
            scanf("%f", a1);
            printf("Podaj a2: ");
            scanf("%f", a2);
            printf("Podaj a3: ");
            scanf("%f", a3);
            printf("Podaj a4: ");
            scanf("%f", a4);
            printf("Podaj a5: ");
            scanf("%f", a5);
            printf("Podaj a6: ");
            scanf("%f", a6);
            printf("Podaj a7: ");
            scanf("%f", a7);
            printf("Podaj a8: ");
            scanf("%f", a8);
            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6) + a7*pow(x, 7) + a7*pow(x, 7);



        //y = pow(x, 2) + 1;
        //area = area + y*dx;
        //printf("x:%f y:%f Area:%f\n",x ,y, area);
        }*/


//switch - obliczanie pola w zależności od potęgi
        switch(potega)
        {
        case 0:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 1:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 2:
           printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 3:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 4:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            printf("Podaj a4: ");
            scanf("%f", &a4);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 5:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            printf("Podaj a4: ");
            scanf("%f", &a4);
            printf("Podaj a5: ");
            scanf("%f", &a5);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 6:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            printf("Podaj a4: ");
            scanf("%f", &a4);
            printf("Podaj a5: ");
            scanf("%f", &a5);
            printf("Podaj a6: ");
            scanf("%f", &a6);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 7:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            printf("Podaj a4: ");
            scanf("%f", &a4);
            printf("Podaj a5: ");
            scanf("%f", &a5);
            printf("Podaj a6: ");
            scanf("%f", &a6);
            printf("Podaj a7: ");
            scanf("%f", &a7);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6) + a7*pow(x, 7);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }
            break;
        case 8:
            printf("Podaj a0: ");
            scanf("%f", &a0);
            printf("Podaj a1: ");
            scanf("%f", &a1);
            printf("Podaj a2: ");
            scanf("%f", &a2);
            printf("Podaj a3: ");
            scanf("%f", &a3);
            printf("Podaj a4: ");
            scanf("%f", &a4);
            printf("Podaj a5: ");
            scanf("%f", &a5);
            printf("Podaj a6: ");
            scanf("%f", &a6);
            printf("Podaj a7: "); 
            scanf("%f", &a7);
            printf("Podaj a8: ");
            scanf("%f", &a8);
            for(x = xp; x<= xk; x = x+dx)
            {


            y = a0*pow(x, 0) + a1*pow(x, 1) + a2*pow(x, 2) + a3*pow(x, 3) + a4*pow(x, 4) + a5*pow(x, 5) + a6*pow(x, 6) + a7*pow(x, 7) + a8*pow(x, 8);
            area = area + y*dx;
        printf("x:%f y:%f pole:%f\n",x ,y, area);
            }


        }
    printf("\nPole pod wykresem wynosi: %f", area);

    //}
    return 0;
