#include<stdio.h>
#include<math.h>
int main()

//TO CALCULATE THE ROOTS OF QUADRATIC EQUATION
{
printf("quadratic equation = ax*2 +bx +c \n");
float a,b,c,root1,root2,disc,real,img,p,q,i;

printf("a = ");
scanf("%f", &a);
printf("b = ");
scanf("%f", &b);
printf("c = ");
scanf("%f", &c);

disc=b*b-4*a*c;
if (disc==0)
{
printf("ROOTS ARE REAL AND EQUAL \n");
root1=-b/(2*a);
root2=-b/(2*a);
printf("ROOT1 = %f \n", root1);
printf("ROOT2 = %f \n", root2);
}
else if (disc>0)
{
printf("ROOTS ARE REAL AND DISTINCT \n");
root1=-b/(2*a) + sqrt(disc)/(2*a);
root2=-b/(2*a) - sqrt(disc)/(2*a);
printf("ROOT1 = %f \n",root1);
printf("ROOT2 = %f \n",root2);
}
else if (disc<0)
{
printf("ROOTS ARE COMPLEX AND DISTINCT \n");
real=-b/(2*a);
img=sqrt(fabs(disc))/(2*a);
printf("ROOT1= %f + i %f \n",real,img);
printf("ROOT2= %f - i %f \n",real,img);
}
return 0;
}
