Zadanie rekrutacyjne 
---

W tym zadaniu poproszę Cię o zrobienie prostej aplikacji internetowej opartej na frameworku React. Zadanie będzie składało się z części głównej, której wykonanie jest niezbędne. Dodatkowo poniżej polecenia głównego dorzucę kilka podpunktów, których wykonanie nie jest niezbędne, ale na pewno pozwoli uzyskać lepszą ocenę koncową. 

Zanim przejdziemy do polecenia, chciałbym zaznaczyć kilka zasad, których należy się trzymać podczas implementacji tego zadania.  

* Wykorzystaj podejście funkcyjne oraz hooki.  

* Wykorzystaj standard ES6 (let, const,  arrow functions itp.) 

* W tworzeniu elementów strony wykorzystaj biblioteki material-ui i/lub styled-components (tak, można korzystać z gotowych komponentów, grunt to potrafić ich świadomie używać, ale też nie zabraniam pisać ich od podstaw, jeśli ktoś ma taką ochotę :D) 

* W przypadku obsługi zapytan do API wykorzystaj bibliotekę axios. 

* Do nawigacji po aplikacji wykorzystaj bibliotekę react-router. 

  

### Na co będę dodatkowo zwracał uwagę

* Czytelność kodu (adekwatne nazewnictwo zmiennych, dobre formatowanie kodu, komentarze itp.) 

* Estetyka (nawet jeśli rozwiązanie jest minimalistyczne to chciałbym, żeby interfejs był schludny) 

* Dobre praktyki korzystania z systemu kontroli wersji git. (Adekwatne nazwy commitów, w przypadku rozbudowy zadania branche feature/branch, fix/branch) 

 

### Zadanie podstawowe 

Wykonaj fork tego projektu. 

Napisz aplikację internetową, która po uruchomieniu na ścieżce _/_ wyświetli cytat pobrany z API (dokumentację API znajdziesz w dalszej części dokumentu). 
Pod cytatem dodaj przycisk, który przekieruje użytkownika do ścieżki _/list_. 
 
Pod ścieżką _/list_ wyświetl listę stworzen pobraną z API. 

Pojedynczy wiersz należy traktować jako osobny byt, który otrzymuje dane do wyświetlenia za pomocą argumentów (props), oraz przetrzymuje je w swoim stanie (podpowiedź, hook useState()). W przypadku pola attributes, wszystkie jego elementy należy wypisać po przecinku. 

Przykładowy układ strony:

![Przykładowy układ strony](https://i.imgur.com/afCZi8M.png)


W podstawowej wersji aplikacji nie wyświetlamy parametru imageURL 

Adres API: https://testapi.bopke.stream

Uproszczona dokumentacja API: 

#### GET /
przykładowa odpowiedź:
```json
{"author":"Ryszard","quote":"Mortimerze, zamieniłem się w ogóra. Jestem Ogór Ryszard."}
``` 

#### GET /beings
przykładowa odpowiedź:
```json
{"beings":[{"id":4,
            "name":"Kicia",
            "type":"Kot",
            "imageURL":"https://i.imgur.com/jllAWBp.png",
            "attributes":["puszysty",
                          "dużo miauczy"]
          }]
}
```

### Podpunkty dodatkowe

1. Wystylizuj tabelę tak by każdy wiersz: 

  * wyświetlał zdjęcie stworzenia wykorzystujące, jako źródło, pobrane z API pole imageURL. 

  * posiadał przycisk, po kliknięciu którego w konsoli wypisze się tekst “Hello from: {imię_stworzenia}”. Imię stworzenia zostanie pobrane bezpośrednio ze stanu wiersza, z poziomu którego przycisk został kliknięty. 

  * wyświetlał elementy pola attributes jeden pod drugim

 

Jeśli chodzi o układ i styl to nie ograniczam. Zależy mi głównie na tym by było to czytelne i estetyczne. 

2. Wystylizuj stronę główną zawierającą cytat (dodaj tło, zmien czcionkę, wystylizuj guzik, itp. itd. daj się ponieść fantazji)  
 
3. Dostosuj strony do wyświetlania na urządzeniach mobilnych (bardzo polecam komponent Grid biblioteki material-ui) 
 
