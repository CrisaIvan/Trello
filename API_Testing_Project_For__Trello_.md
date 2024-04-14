<h1>API Testing Project for Trello</h1>

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: Trello

Tools used: Postman

Collection link: https://red-zodiac-950716-1.postman.co/workspace/CristinaTMTA11~b83ba4f1-693b-4f60-b0e3-f9b3cb38ffda/collection/30261120-c0975692-c837-4b40-afa0-836a003994d2?action=share&creator=30261120

<h2>Tests performed</h2>

<ol>
<li>**Get Board**</li>

HTTP method for request: GET <br>
Request description: Request a single board<br>
Test types / techniques used: Testare functionala<br>
Response status code: Status code 200 <br>

Below you can find a picture of the API request from Postman:<br>

[D:\1.Tester\TM\Proiect Trello\GET body snip.PNG]<br>

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

**Inserati aici concluziile pe care le-ati obtinut in urma executarii testelor si introduceti informatii cum ar fi cate teste au fost create si executate, ce procentaj aproximativ din cerintele in scop au fost acoperite, daca exista vreo functionalitate pe care nu ai apucat sa o testezi, daca bug-urile gasite impacteaza lansarea produsului in productie sau se pot fixa si ulterior, daca ai identificat riscuri de produs care trebuie mitigate, daca e vreo reecomandare pe care vrei sa o faci pentru lansare, daca sunt ceva lessons learned de care trebuie sa se tina cont la proiectele viitoare etc**

[def]: <GET body snip.PNG>