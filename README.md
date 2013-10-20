#rozwiazania

zad 1 (w miejsce kropek '...' wpisz kod tak aby powstal dzialajacy program /*program wypisuje liczby z tablicy tabela []
w w odwrotenj kolejnosci, tj 12,6,4,2,1.)

```c
int main () {
int i;
int tabela[]={1,2,4,6,12}
for(i=4; i>=0; i=i-1)
printf("%i",tabela [i]
return 0;
}
```

zad 2 program ktory wypisuje kolejne liczby potego 2 az do 2010 
       a) uzywajac petli for
       
       
       b) uzywajac petli "while"
'''c
main () {
  int a;
  a=1;
  while (a<=2010){
  printf("%i \n" ,a);
  a=a*2;}
}
'''
