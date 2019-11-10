# terminacom
Elaborar em programa que, considerando os valores inteiros A e B, verifique se o numero B esta contido entre os ultimos algarismos de A
import java.util.Scanner;
/*Elaborar em programa que, considerando os valores inteiros A e B, verifique se o numero B esta contido entre os
ultimos algarismos de A*/
public class terminacom {
public static void main(String[] args) {
// TODO Auto-generated method stub
int a, b, resto=10, num=0;
Scanner get = new Scanner(System.in);
System.out.println("Digite um valor para A");
a = get.nextInt();
System.out.println("Digite um valor para B");
b = get.nextInt();
while(num < b)
{
num=a%resto;
resto*=10;
}
if (num==b)
System.out.println("O valor de B esta contido em A");
else
System.out.println("O valor de B não esta contido em A");
}
}
