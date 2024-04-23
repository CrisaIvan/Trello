# API Testing Project for Trello

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

<b>Application under test</b>: Trello

<b>Tools used</b>: Postman

<b>Collection [link](https://red-zodiac-950716-1.postman.co/workspace/CristinaTMTA11~b83ba4f1-693b-4f60-b0e3-f9b3cb38ffda/collection/30261120-c0975692-c837-4b40-afa0-836a003994d2?action=share&creator=30261120)</b>

## Tests performed

### 1. Get Board

- _HTTP method for request:_ GET
- _Request description:_ Request a single board
- _Test types / techniques used:_ Testare functionala
- _Response status code:_ Status code 200 

Below you can find a picture of the API request from Postman:<br>

<img width="647" alt="p1" src="https://github.com/CrisaIvan/Trello/assets/64869220/42f1f9a0-8b57-4001-8f85-79ea7fb18f4e">


JavaScript Tests:

[D:\1.Tester\TM\Proiect Trello\GET test snip.PNG]

<br>

<li>Create Board</li>

HTTP method for request: POST <br>
Request description: Create a new board<br>
Test types / techniques used: Testare functionala<br>
Response status code: Status code 200<br>

Below you can find a picture of the API request from Postman:<br>

[D:\1.Tester\TM\Proiect Trello\POST body.JPG]<br>

JavaScript Tests:

[D:\1.Tester\TM\Proiect Trello\POST test.JPG]<br>

.............

<li>Create TO DO list</li>

HTTP method for request: POST<br>
Request description: Create a new List on a Board<br>
Test types / techniques used: Testare functionala<br>
Response status code: Status Code 200<br>

Below you can find a picture of the API request from Postman:<br>

[D:\1.Tester\TM\Proiect Trello\POST TO DO Body.JPG]<br>

JavaScript Tests:

[D:\1.Tester\TM\Proiect Trello\POST TO DO tests.JPG]<br>

</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>

**Inserati aici o poza cu raportul de executie din Postman**<br>

The collection was also run through newman directly from the terminal, and the results can be found below:<br>

**Inserati aici o poza cu raportul de executie din Newman**<br>

<h2>Defects found</h2>

The following issues were identified while running the postman tests:<br>

\***\*Inserati aici fie un fisier pdf care sa contina raportarea tuturor bug-urilor, fie le descrieti direct in git
Bug-urile trebuie sa contina titlu, preconditii, pasi de executie, rezultate asteptate si rezultate actuale.
Optional, bug-urile pot fi raportate in jira, si apoi puteti pune poze direct din jira**

<h2>Conclusions</h2>
In total au fost create si executate 17 teste in felul urmator: 

a) doua  teste pentru testare negativă  &#10004;
- punem intenționat idList greșit pentru a testa dacă sistemul reacționează corespunzător:
- punem intenționat valoarea greșită (1) pentru card number pentru a testa dacă sistemul reacționează corespunzător:

b) 14 teste pentru testare pozitiva &#10004;

c) un test pentru Testare de performanță: &#x274c;
- Testul este failed pentru că timpul de răspuns este mai mare de 200ms. Ajustarea timpul la 400ms face ca testul sa fie passed.
