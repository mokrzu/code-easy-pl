# Terminalowa lista to-do.

**Poziom**: podstawowy.

**Wymagania**: wcześniejsza styczność z Ruby oraz pracą w konsoli.

---

Zawartość przewodnika:

1. **Cel ćwiczenia**
2. **Opis zadania**
3. **Lista kroków**
4. **Wymagane struktury oraz metody**
5. **Rozwiązania problemów**
6. **Linki do dokumentacji**
7. **Zgłaszanie problemów i uwag**

---

## Cel ćwiczenia.

Tym razem, przewodnik skupi się na podstawowych aspektach pisania programu. 

Pomijając dodatek algorytmicznych zagadek. 

Tak więc wykorzystamy pętle, warunki, proste  wejście/wyjście (danych do/z programu), 
zmienne, tablice a także użyjemy zewnętrznej biblioteki (gema).
Czyli podstawowe narzędzia każdej osoby tworzącej kod.  

Pomimo długiej listy wymienionych elementów, nasz program będzie bardzo krótki i szybki do napisania, 
w przybliżeniu 30-kilka linii kodu. 
Niemniej jednak wykonanie ćwiczenia do końca, z pewnością zwiększy wiele umiejętności:) 

---

## Opis zadania.

### Treść.

Terminalowa lista to-do, to prosty program do przechowywania listy zadań.
Użytkownik może wybrać operację dodawania/usuwania/wyświetlania/wyjścia z programu, 
przy pomocy wprowadzonego z klawiatury polecenia. (może to być 1 litera lub cały wyraz)

Dodając zadanie, wymagane jest jedynie, podanie jego treści. 

Wyświetlając wszystkie zadania, użytkownik otrzymuje listę w której każdemu zadaniu jest przyporządkowany jego numer. 
(oznaczający pozycję w tablicy, jednak numeracja w wyświetlanej liście będzie zaczynać się od jedynki)

Usuwanie zadania polega na podaniu numeru, zadania do usunięcia, z listy wszystkich zadań.
Podanie polecenia wyjścia, przerywa główną pętlę programu, tym samym kończąc jego działanie.

Na koniec, do naszej aplikacji dodamy kolorowanie tekstu.

Gra powinna działaś z poziomu konsoli, tzn. po uruchomieniu skryptu `ruby todo.rb.`
Skrypt(czyt. program) oczywiście należy utworzyć samodzielnie.  

Jak można zauważyć zadania będę przechowywane tak długo jak działa nasz program, trwałym zapisywaniem danych zajmiemy się w kolejnych przewodnikach.

### Przykład działania.

![script screenshot](http://cloud.github.com/downloads/mokrzu/code-easy-pl/todolist.png)

---

## Lista kroków.

### Wstępne uwagi.

Po pierwsze, warto przypomnieć sobie uwagi z [poprzedniego tutoriala.](http://documentup.com/mokrzu/code-basics-pl#lista-krokow/proces-pisania-programu)

Po drugie, należy pamiętać że Ruby jest dość rozbudowanym językiem. 
Dlatego dane zadanie można wykonać na wiele sposobów.  
Oczywiście szukając odpowiednich rozwiązań, najlepiej wybierać te które najlepiej rozumiemy i potrafimy dostosować do naszych potrzeb.  
W chwili gdy już otrzymamy działającą aplikację, można eksperymentować z alternatywnymi sposobami implementacji.

### Opis kroków.
*Tym razem, nie narzucam kolejności wykonania poszczególnych kroków. 
Istnieje kilka poprawnych sposobów ponumerowania wymienionych zadań.*

*   **Główna pętla.** Użyj pętli ``while``, do aby ciągle pobierać polecenia od użytkownika. Pętla powinna zostać przerwana, gdy użytkownika wyda polecenie oznaczające zakończenie programu.

*   **Deklaracja zmiennych.** Przygotowanie zmiennej w której będziemy trzymali komendę wprowadzoną przez użytkownika.  Będzie ona służyła do sprawdzenia które zadanie powinniśmy wykonać, a także do przerwania wykonywania głównej pętli programu. Zadania przechowuj w przygotowanej wcześniej pustej tablicy.

*   **Usunięcie zadania**. Znając indeks zadania w tablicy, wykorzystaj metodę ``delte_at`` w celu usunięcia danego elementu. Pamiętaj że w tablicy numeracja zaczyna się od 0.

*   **Wejście/Wyjście.** Wyświetlaj instrukcje dla użytkownika,  oraz pobieraj polecenia i nowe zadania. Czytając tekst podany z klawiatury, pamiętaj że na jego końcu znajduje się znak nowej linii "\n". Użyj odpowiedniej metody, aby go usunąć.

*   **Sprawdzanie polecenia**. Wykorzystaj instrukcje warunkowe, w celu wykonania odpowiednich procedur w zależności od komendy podanej przez użytkownika.

*   **Wyświetlenie listy zadań**.  Wypisanie ponumerowanych zadań można osiągnąć na kilka sposobów, najszybszy z nich to wykorzystanie iteratora ``each_with_index``.

*   **Dodaj gem kolorujący tekst**.  Prosty gem (biblioteka) ‘colorize’ posiada metody pozwalające w łatwy sposób zmieniać kolor tła i tekstu.


---

## Wymagane struktury oraz metody.


---

## Rozwiązania problemów.


---

## Linki do dokumentacji.

Oficjalna, mało zachcająca strona bibloteki. Jednak posiada spis przykładowych zastosować modułu:
[Colorize usage samples.](http://colorize.rubyforge.org/files/README_txt.html)

Na stackoverflow można spotkać bardzo dużo merytorycznych odpowiedzi. 
Jeżli masz z czymś problem, prawdopodobnie ktoś już o to spytał.
[Another colorize usage sample.](http://stackoverflow.com/questions/1489183/colorized-ruby-output?answertab=votes#tab-top)

Oficjalna dokumentacja, przydatna gdy chcemy znaleźć opis działania konkretnej metody:
[Array - Ruby documentation.](http://www.ruby-doc.org/core-1.9.3/Array.html)

RubyMonk - praktyczne ćwiczenia z podstaw języka:
[Arrays introduction, ](http://rubymonk.com/learning/books/1/chapters/1-arrays/lessons/2-arrays-introduction)
[if-else statement.](http://rubymonk.com/learning/books/1/chapters/8-control-structures/lessons/41-conditions-using-the-if-statement)

Ćwiczenia z "Learn Ruby the Hard Way". Powiązane tematycznie z naszym zadaniem:

1.  [String and Text.](http://ruby.learncodethehardway.org/book/ex6.html)
2.  [Asking Questions.](http://ruby.learncodethehardway.org/book/ex11.html)
3.  [What if?](http://ruby.learncodethehardway.org/book/ex29.html)
4.  [Else and if.](http://ruby.learncodethehardway.org/book/ex30.html)
5.  [Accessing Elements Of Arrays.](http://ruby.learncodethehardway.org/book/ex34.html)
6.  [While Loops.](http://ruby.learncodethehardway.org/book/ex33.html)


---

## Zgłaszanie problemów i uwag.

Tymczasowo, uwagi oraz problemy można zgłaszać, przez opcję [Issues](https://github.com/mokrzu/code-basics-pl/issues) na Github
lub bezpośrednio do mnie - Łukasz.
