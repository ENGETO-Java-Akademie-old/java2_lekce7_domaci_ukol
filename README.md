

# Java2 - Lekce 7 Domaci ukol

V sedmé lekci jsme si ukázali základ třídy, která pomocí anotací a reflexe umožní zapisovat soubory v CSV formátu do souboru. V domácím úkolu se k tomu vrátíme a úkolem bude takovou knihovnu doplnit a rozšířit.

1. Navrhněte API pro knihovnu, tak jak vám přijde takovou knihovnu používát.
1.1 Metoda na zápis do souboru (do kterého souboru, v jakém formátu, vypsat i hlavičku nebo ne, jak ošetřit vyjímky)
1.2 Anotace pro úpravu chování (formát čísla, formát datumu, upper case, lower case)
2. Doplntě požadovanou funkcionality dané knihovny
3. Ošetřete vyjímky a vyzkoušejte chování
3.1 Zapisovaný objekt je null
3.2 Do daného souboru nejde zapisovat

## Hint

1. Pro formát čísel použijte `String.format()` https://dzone.com/articles/java-string-format-examples

```
Double x = 12.456;
String text = String.format("%.2f", x);
System.out.println(text); //12.46

```

2. Pro formát datumu použijte SimpleDateFormat https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html

```
String pattern = "yyyy-MM-dd";
SimpleDateFormat simpleDateFormat = new SimpleDateFormat(pattern);

Data date = new Date();

String text = simpleDateFormat.format(date);
System.out.println(text); // 2021-05-19
```

