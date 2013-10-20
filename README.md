#rozwiazania

zad 1 (w miejsce kropek '...' wpisz kod tak aby powstal dzialajacy program /*program wypisuje liczby z tablicy tabela []
w w odwrotenj kolejnosci, tj 12,6,4,2,1.).

```c
int main () {
int i;
int tabela[]={1,2,4,6,12}
for(i=4; i>=0; i=i-1)
printf("%i",tabela [i]
return 0;
}
```

zad 2 program ktory wypisuje kolejne liczby potego 2 az do 2010.
       a) uzywajac petli for
```c
main () {
  int a=1;
  for (a=1; a<=2010; a=a*2)
    printf ("%i \n", a);
}
```
       
       b) uzywajac petli "while"
```c
main () {
  int a;
  a=1;
  while (a<=2010){
  printf("%i \n" ,a);
  a=a*2;}
}
```

zad 3 napisac i urochomic program w C, ktory wczytuje liczbe naturalna "n" i drukuje wartosci kwadratow.
```c
main () {
  int n,suma,i;
  suma=0;
  printf("Podaj liczbe \n");
  scanf("%i", &n);
  for (i=1; i<=n; i++)
    suma=suma+i*i;
  printf("wynik sumy to: %i\n" ,suma);
	 }
```

zad4 napisac program obliczajacy wartosc kazdego z ponizszych wyrazen.
```c
main () {
  int n1,n2,n3;
    n1=5+3*8/2-3;
  printf("n1 wynosi: %i \n",n1);
  n2=2%2+2*2-2/2;
  printf("n2 wynosi: %i \n",n2);
  n3=2*4*(5+9/2);
  printf("n3 wynosi: %i \n",n3);
}
```

zad5 Program po podaniu liczby wyswietla ta liczbe, jej kwadrat i szescian.
```c 
main(){
  int i;
  printf("podaj liczbe \n");
  scanf("%i", &i);
  printf(" Podana liczba to: %i \n Kwadrat tej liczby to: %i \n Sześcian tej liczby to: %i \n", i, i*i, i*i*i);
}
```

zad 6 ????
```c
main() {
  int n,suma;
  n=1;
  suma=0;
  for(n=1; n<31; n=n+1){
    if{ (n<16)
  printf ("Aktualna liczba to:%i \n",n);

    else{ 
 printf("Aktualna liczba to:%i \n", n*2);
    }
    }
}
}
```

zad7 Program wyliczajacy sume, roznice, iloczyn i iloraz po podaniu dwoch liczb
```c
main(){
  int i,j;
  printf("Podaj pierwsza liczbę \n", i );
  scanf("%i",&i);
  printf("Podaj druga liczbe  \n",j);
  scanf("%i",&j);
  printf("suma to: %i \n roznica to: %i \n iloczyn to: %i \n iloraz to: %i \n",i+j, i-j, i*j, i/j);
}
```

zad8 Program ktory zaczyta liczbe w syst dziesietnym a wyswietli w binarnym
```c
main(){
int liczba=9;
int i;
int wynik[20];
/*printf("Podaj liczbę w systemie 10");*/
/*scanf("%i",&liczba);*/
i=0;
while(liczba!=0)
{
    wynik[i]=liczba%2;
    printf(" RESZTA %i przez 2 = %i ",liczba,wynik[i]);
    liczba=liczba/2;
    printf(" PO PODZIELENIU LICZBA =  %i \n", liczba);
    i++;
}
printf("\nWYNIK:");
for(i=i-1;i>=0;i--) printf(" %i ",wynik[i]);


}
```
