# CarRegistrationNumber -PersonalProject- -DEMOVERSION-

Aplicatie realizata pe versiunea de Android Oreo 8.1 ( API 27 ).

Aceasta aplicatie preia un numar de inmatriculare introdus intr-un PlainText si se verifica daca se afla in baza de date ( Obs: Momentan "Baza de date" reprezinta un LinkedHasMap unde cheia este un "String" ce reprezinta numarul de inmatriculare iar valoarea este un Boolean ce indica daca masina cu acel numar de inmatriculare are sau nu asigurare ) . 
Verificarea se face printr-un buton , iar rezultatele ( indicate de un mesaj(AlertDialog) ) pot fi urmatoarele  :
- "Numarul de inmatriculare este gresit". Numarul de inmatriculare al unei masini , din Romania , este format din 7 caractere ( 5 litere si 2 numere ) .Prin urmare , daca se va depasi acel numar de caractere , vom primi acel mesaj de eroare.
- "Va rugam introduceti numarul de inmnatriculare" . Acest mesaj va aparea in momentul in care nu introducem nimic in PlainText .
- "Masinuma cu numarul de inmatriculare XX00XXX nu exista in baza de date" . Cum am zis mai sus , baza de date reprezinta un LinkedHasMap care este populat cu cateva numere de inmatriculare . Aceste mesaj va aparea in momentul in care numarul de inmatriculare introdus nu exista in acel LinkedHasMap.
- "Masinuma cu numarul de inmatriculare XX00XXX nu are asigurare" . Acest mesaj va aparea in momentul in care valoarea atribuita numarului de inmatriculare este "false" . 
- "Masinuma cu numarul de inmatriculare XX00XXX are asigurare" . Acest mesaj va aparea in momentul in care numarul de inmatriculare se afla in baza de date si valoarea acestuia este "true" . Pentru acele masini care au asigurare , se poate vizualiza data expirarii acesteia fiind reprezentat de un ArrayList . Legatura dintre "Baza de date" reprezentata de un LinkedHashMap si ArrayList-ul ce reprezinta datele de expirare ale asigurarilor s-a realizat tot printr-un LinkedHasMap unde cheia reprezinta primul LinkedHasMap ("Baza de date") iar valoarea este ArrayList-ul.

Proiectul este abia inceput , avand inca cateva probleme , cum ar fi selectarea datei de expirare a asigurarii pentru numarul de inmatriculare respectiv.

Dezvoltarea pe viitor al proiectului reprezinta :
- Utilizarea bazelor de date
- Posibilitatea de a crea o asigurare 
