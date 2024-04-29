# API Testing Project for Trello

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

<b>Application under test</b>: Trello

<b>Tools used</b>: Postman

<b>Collection [link](https://red-zodiac-950716-1.postman.co/workspace/CristinaTMTA11~b83ba4f1-693b-4f60-b0e3-f9b3cb38ffda/collection/30261120-c0975692-c837-4b40-afa0-836a003994d2?action=share&creator=30261120)</b>

## Tests performed

### 1. Get Board

- _HTTP method for request:_ GET
- _Request description:_ Request a single board
- _Test types / techniques used:_ Functional testing.
- _Response status code:_ Status code 200 

Below you can find a picture of the API request from Postman:<br>

<img width="647" alt="p1" src="https://github.com/CrisaIvan/Trello/assets/64869220/42f1f9a0-8b57-4001-8f85-79ea7fb18f4e">


JavaScript Test (Passed):

- "Status code is 200"

![GET test snip](https://github.com/CrisaIvan/Trello/assets/95541889/351b9f3a-baf0-4d51-aba2-4335ac7af345)



### 2. Create Board

- _HTTP method for request:_ POST
- _Request description:_ Create a new board
- _Test types / techniques used:_ Functional testing. Prin testele efectuate s-au verificat urmatoarele: daca boardul a fost creat, daca board-ul este privat si daca obiectul numit „calendar” este dezactivat.
- _Response status code:_ Status code 200

Below you can find a picture of the API request from Postman:<br>

![Create Board- body](https://github.com/CrisaIvan/Trello/assets/95541889/c8b44610-bb98-4223-bcc6-5a4cbe42b897)

JavaScript Tests (Passed):
- "Status Code is 200"
- "Board-ul este creat"
- "Board-ul este privat"
- "Calendarul este dezactivat"
   
![Create Board- test](https://github.com/CrisaIvan/Trello/assets/95541889/ecb72fc3-69af-463f-8d9e-cca3e89cbee7)


### 3. Create TO DO List

- _HTTP method for request:_ POST
- _Request description:_ Create a new TO DO List on a Board
- _Test types / techniques used:_ Functional testing. Prin testele efectuate s-au verificat urmatoarele: numele listei este "TO DO", lista este deschisa si lista se afla in interiorul board-ului corect.
- _Response status code:_ Status Code 200

Below you can find a picture of the API request from Postman:<br>

![TODO list - Body](https://github.com/CrisaIvan/Trello/assets/95541889/5448d7f5-a432-408f-846d-7601ab05a027)


JavaScript Tests (Passed):
- "Status Code is 200"
- "Lista TO DO este creata"

![TODO list - Test](https://github.com/CrisaIvan/Trello/assets/95541889/ca031b1c-810c-4f1a-a26d-41ffc2d4a708)

### 4. Create DONE List

- _HTTP method for request:_ POST
- _Request description:_ Create a new DONE List on a Board
- _Test types / techniques used:_ Functional testing. Prin testele efectuate s-au verificat urmatoarele: numele listei este "DONE", lista este deschisa si lista se afla in interiorul board-ului corect.
- _Response status code:_ Status Code 200

Below you can find a picture of the API request from Postman:<br>

![DONE list - Body](https://github.com/CrisaIvan/Trello/assets/95541889/e3c478a2-b336-4135-a046-4aedcdc060ab)

JavaScript Tests (Passed):
- "Status Code is 200"
- "Lista DONE este creata"

![DONE list - Test](https://github.com/CrisaIvan/Trello/assets/95541889/865c856a-3fde-43f2-ba13-d0ebb2d92fe0)

### 5. Create New Card

- _HTTP method for request:_ POST
- _Request description:_ Create a new card. 
- _Test types / techniques used:_ Functional testing. Prin testele efectuate s-au verificat urmatoarele: numele card-ului este cel asteptat ("Sign-up for Trello" in acest caz), card-ul este creat in interiorul listei TO DO corespunzatoare, card-ul este creat in interiorul board-ului corespunzator, cardul are proprietatea 0.
- _Response status code:_ Status Code 200

Below you can find a picture of the API request from Postman:<br>

![New Card - Body](https://github.com/CrisaIvan/Trello/assets/95541889/3eec8ede-23b3-4a2b-a0a2-63b99c161d6a)


JavaScript Tests (Passed):
- "Status Code is 200"
- "Cardul este creat"
  
![New Card - Test](https://github.com/CrisaIvan/Trello/assets/95541889/9f6eaebe-07aa-4fe1-a697-4bca798177c6)

### 6. Move Card

- _HTTP method for request:_ PUT
- _Request description:_ Update a card. Move a Card from TO DO List to DONE List.
- _Test types / techniques used:_ Functional testing. Prin testele efectuate s-au verificat urmatoarele: numele card-ului este acelasi ("Sign-up for Trello"), cardul a fost mutat in lista DONE. O modalitate de a verificare este sa schimbam, in interiorul testului, variabila "doneListID" cu "todoListID". Vom obtine eroare, ceea ce arata ca acesta a fost intr-adevar mutat; Non-functional testing: Se verifica daca timpul de răspuns este mai mare de 200ms.
- _Response status code:_ Status Code 200

Below you can find a picture of the API request from Postman:<br>

![Move Card - body](https://github.com/CrisaIvan/Trello/assets/95541889/cfc47658-6eb1-4a07-bac7-8732576c98be)


JavaScript Tests (Passed):
- "Status Code is 200"
- "Card-ul este mutat"
- "Timpul de raspuns este mai mic de 400ms"

![Move Card - Test](https://github.com/CrisaIvan/Trello/assets/95541889/6e999079-9258-421d-8143-9cf2a03ba7e4)


</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>


![raport de executie](https://github.com/CrisaIvan/Trello/assets/95541889/2b0eb64f-08af-4b1b-be04-788dfb5fec01)


<h2>Conclusions</h2>
In total au fost create si executate 17 teste in felul urmator: 

a) doua  teste pentru testare negativă  &#10004;
- punem intenționat idList greșit pentru a testa dacă sistemul reacționează corespunzător:
- punem intenționat valoarea greșită (1) pentru card number pentru a testa dacă sistemul reacționează corespunzător:

b) 14 teste pentru testare pozitiva &#10004;
- "Status code is 200" a fost rulat fiecare dintre request-urile: Get Board, Create Board, Create TO DO List, Create DONE List, Create Card, Move Card;
- "Board-ul este creat";
- "Board-ul este privat";
- "Calendarul este dezactivat";
- "Lista TO DO este creata";
- "Lista DONE este creata";
- "Card-ul este creat";
- "Card-ul este mutat";
- "Timpul de raspuns este mai mic de 400ms".
  
c) un test pentru Testare de performanță: &#x274c;
- Testul este failed pentru că timpul de răspuns este mai mare de 200ms. Ajustarea timpul la 400ms face ca testul sa fie passed.
