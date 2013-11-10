#rozwiazania

zad 1 (w miejsce kropek '...' wpisz kod tak aby powstal dzialajacy program /*program wypisuje liczby z tablicy tabela []
w w odwrotenj kolejnosci, tj 12,6,4,2,1.).

```c
int main () {
int i;
int tabela[]={1,2,4,6,12}
for(i=4; i>=0; i=i-1)
printf("%i",tabela [i]);
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
    if (n<16)
    {
  printf ("Aktualna liczba to:%i \n",n);
  else
  { 
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
for(i=i-1; i>=0; i--) 
printf("%i", wynik[i]);
}
```

zad10 Napisac program ktory  wczyta liczbe calkowita i wypisze czy jest wieksza od 5
```c
main () {
  int i;
  printf("Podaj liczbe: \n");
  scanf("%i", &i);
  if (i>=5)
    printf("Twoja liczba jest wieksza lub rowna od 5 \n");
    else 
    printf("Twoja liczba jest mniejsza od 5 \n");
}
```
zad11 Napisac program ktory wczyta liczbe calkowita i wypisze czy jest dodatnia, ujemna czy rowna 0.
```c
main () {
  int i;
  printf("Podaj liczbe calkowita: \n");
  scanf("%i", &i);
    if(i>0)
        printf("Twoja liczba jest dodatnia \n");
    else if (i<0)
              printf("Twoja liczba jest ujemna \n");
         else
              printf("Twoja liczba jest rowna 0 \n");
}
```

zad12 Wczyta liczbe calkowita i wypisze czy liczba jest parzysta czy nie.
```c
main () {
  int i;
  printf("Podaj liczbe calkowita: \n");
  scanf("%i", &i);
  if (i%2)
    printf("Twoja liczba jest nieparzysta\n");
  else 
  printf("Twoja liczba jest parzysta \n");
}
```

zad13 Wczyta dwie liczby calkowite i wypisze czy sa rowne.
```c
main () {
  int i, j;
  printf("Podaj pierwsza liczbe \n");
  scanf("%i", &i);
  printf("Podaj druga liczbe \n");
  scanf("%i", &j);
  if (i==j)
    printf("Twoje liczby sa rowne\n");
  else 
    printf("Twoje liczby nie sa rowne\n");
}
```

zad14  Wczyta 2 liczby calkowite i wypisze ktora z nich jest wieksza
```c
main () {
  int i, j;
  printf("Podaj pierwsza liczbe: \n");
  scanf("%i", &i);
  printf("Podaj druga liczbe: \n");
  scanf("%i", &j);
  if (i>j)
    printf("Twoja pierwsza liczba jest wieksza \n");
    else 
    printf("Twoja druga liczba jest wieksza \n");
}
```
zad15 Obliczy i wypisze na ekran sume kwadratow liczb od 1 do 20
```c
main () {
  int suma, i;
  suma=0;
  for(i=1; i<=20; i++)
    suma=suma+i*i;
  printf("Suma kwadratow liczb od 1 do 20 to: %i\n", suma);
}
```

zad16 Wczytuje liczbe calkowita n>=0 a nastepnie n liczb rzeczywistych (double %lf) i drukuje te liczby w trzech
kolumnach w taki sposob, zeby zachowac krycie  (tzn. kropka dziesietna zawsze byla w tych samych kolumnach) np gdy
uzytkownik: 
poda 7 0.12 -31,5 2,5 -59,01 26,4 -12,0 8,3 
  kol1    kol2    kol3
  0,12  -31,50    2,50
-59,01   26,40  -12,00
  8,3
  
  Mozna zakładac ze liczby naleza do przedzialu (-100,100).
  Zeby wydrukowal l. rzeczywista na o dl. 6 znakow z 2 cyframi po kropce nalezy w komendzie "printf" uzyc formatu
  "%6.2 lf"      
  
  ./zad < plik_z_danymi --> przekierowuje nas do pliku z danymi np. "n"
  
```c
main () {
  int i, n;
  printf("Podaj liczbe calkowita \n");
  scanf("%i", &n);
  /*deklaracja tablicy*/
  double tab[n];
    /*petla wczytujaca dane do tablicy*/
    for (i=0; i<n; i++)
      scanf("%lf", &tab[i]);
  /*petala wypisujaca dane z tablicy*/
    for (i=0; i<n; i++)
      {
    printf("%2.2lf \n", tab[i]);
    if (i%3==2)
      printf("\n");
 }
}
```
zad17 zadeklaruje tablice 5 liczb calkowitych w nastepujacy sposob: int tab[]={1,3,7,8,9{,
a nastepnie wypisze na ekran jej zawartosc w odwrotnej kolejnosci.
```c
main () {
  int tabela[]={1,3,7,8,9};
  int i;
  for (i=4; i>=0; i=i-1)
    printf("%i\n", tabela[i]);
}
```

zad18 Wczyta od uzytkownika dane do piecioelemntowej tablicy liczb calkowitych a nastepnie wypisze na 
ekran sume jej elementow.
```c
main () {
  int i, j, suma;
  suma=0;
  //wczytywanie ilosci liczb
  printf("Podaj liczbe calkowita \n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tab[j];
  //wczytywanie liczb do tablicy
  for (i=0; i<j; i++)
    scanf("%i", &tab[i]);
  //wczytywanie liczb do tablicy
  for (i=0; i<j; i++){
    //printf("%i \n", tab[i]);
    suma=suma+tab[i];
  }
  //wyswietlanie wyniku
  printf("Wynik to %i \n", suma);
  
}
```

zad19 Wczyta od uzytkownika dane do piecioelemntowej tablicy liczb calkowitych a nastepnie przestawi jej pierwszy
element z ostatnimi i wypisze cala tablice na ekran.
```c
main () {
  int i, j, tmp;
  //wczytywanie liczby elementow tablicy
  printf("Podaj liczbe calkowita: \n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tab[j];
  //wczytywanie danych do tablicy
  for(i=0; i<j; i++)
    scanf("%i", &tab[i]);
  //zamiana pierwszego i piatego elementu tablicy
  tmp=tab[0];
  tab[0]=tab[4];
  tab[4]=tmp;
  //drukowanie elementow tablicy
  for(i=0; i<j; i++)
	printf("%i \n", tab[i]);
  
}
```
zad20 Zadeklaruje dwie piecioelementowe tablice liczb calkowitych, wczyta dane do pierwszej tabel, a nastepnie
przekopijuje dane do drugiej i wypisze na ekran zawartosc drugiej tabeli.
```c
main () {
  int i, j, tmp;
    printf("Podaj liczbe \n");
  scanf("%i", &j);
  //deklaracja pierwszej tablicy
  int tablica[j];
    //deklaracja drugiej tablicy
  int tab[j];
  //petla wczytujaca dane do tablicy pierwszej
  for (i=0; i<j; i++)
    scanf("%i", &tab[i]);
  //petla kopiujaca dane z "tab" do "tablicy"
  for (i=0; i<j; i++) 
 tablica[i]=tab[i];
  //petla wypisujaca dane z tablicy
  for(i=0; i<j; i++)
    {
      printf("tablica[%i]=%i \n",i, tablica[i]);
      }
} 
```
zad21 Napisac program w c sprawdzajacy czy dana liczba jest pierwsza.
```c
main () {
  int i, j, k;
  k=0;
printf("Podaj liczbe: \n");
scanf("%i", &i);
// liczy ilosc dzielnikow
 for(j=1; j<=i; j++)
   if (i%j==0)
     k=k+1;
 //wypisuje liczby ktore maja tylko 2 dzielniki
 if (k==2)
printf("Podana liczba jest pierwsza \n");
else
printf("Podana liczba nie jest pierwsza \n");
}
```

zad22 Napisac program, ktory dla liczby M podanej z klawiatury ma obliczyc najmniejsza liczbe n taka jak 
1+2+3+...+n>=M
```c
main () {
  int i, n, suma;
  n=0;
  suma=0;
  printf("Podaj liczbe: \n");
  scanf("%i", &i);
  while(suma<i)
    {
      n=n+1;
      suma=suma+n;
  }
  printf("szukana liczba to %i \n", n);
}
```
zad23 napisac program ktory dla liczby podanej z klawiatury wypisuje wszystkie jej dzielniki.
```c
main () {
  int i, j, k;
  k=0;
printf("Podaj liczbe: \n");
scanf("%i", &i);
// liczy ilosc dzielnikow
 for(j=1; j<=i; j++)
   if (i%j==0) //sprawdza czy j jest dzielnikiem i.
     //wypisuje dzielniki.
     printf("%d jest dzielnikiem %d \n", j ,i);
}
```
zad24 napisac program ktory zamienia liczbe z systemu dziesietnego na 
a) dwojkowy 
b) osemkowy 
c) szesnatstkowy.

a) Patrz wyzej ;)

b)
```c
main () {
  int i;
  int j;
  int tab[20];
  int k;
  printf("podaj liczbe w systemie 10: \n");
  scanf("%i", &i);
  j=0;
  while (i>0)
    {
      tab[j]=i%8;
      printf("Reszta %i przez 8 = %i", i,tab[j]);
      i=i/8;
      printf(" Liczba po dzieleniu = %i \n", i);
      j++;
    }
  printf("\n wynik:");
  for(k=j-1; k>=0; --k)
    printf("%d", tab[k]);
}
```
zad25 jaka jest roznica powmiedzy j=i++ a  j=++i
