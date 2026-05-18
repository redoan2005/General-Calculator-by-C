# General-Calculator-by-C
#include <stdio.h>
    int add(int a,int b){
    return a+b;
    }
    int subtract(int a,int b){
    return a-b;
    }
    int multiply(int a,int b){
    return a*b;
    }
    float divide(int a,int b){
    if(b!=0)
    return (float) a/b;
    else{
    printf("Math Error");
    return 0;    
    }
    }
    
        int main(){    
    int choice,x,y;
    char cont='y';
    while(cont =='y'|| cont =='Y'){
        printf("\nSimple Calculator\n1.Add\n2.Subtract\n3.Multiply\n4.Divide\n");
        printf("Choose one opetator");
        scanf("%d",&choice);
        printf("enter two values\n");
        scanf("%d %d",&x,&y);
        switch(choice){
            case 1:
            printf("Result is %d\n",add(x,y));
            break;
            case 2:
            printf("Result is %d\n",subtract(x,y));
            break;
            case 3:
            printf("Result is %d\n",multiply(x,y));
            break;
            case 4:
            printf("Result is %.2f\n",divide(x,y));
            break;
            default:
            printf("Not available now\n");
            }
       printf("Do you wanna continue?(y/n)");
       getchar();
       scanf("%c",&cont);
        }
        printf("Thanks for using");
    return 0;
    }
