# Proiect-Java
Posibilitati de Utilizare a Proiectului

Managementul utilizatorilor:

Aplicația permite gestionarea utilizatorilor, care include probabil funcționalități precum crearea, citirea, actualizarea și ștergerea înregistrărilor utilizatorilor.

Interfață web:

Prezența șabloanelor HTML (de exemplu, index.html, user_form.html, users.html) indică faptul că aplicația are o interfață web pentru interacțiunile utilizatorilor. Utilizatorii pot accesa aplicația printr-un browser web.

API RESTful:

Controloarele (de exemplu, UserController.java) sugerează că aplicația poate expune punctele finale RESTful pentru gestionarea utilizatorilor, permițând integrarea cu alte aplicații sau servicii.
Caracteristici Spring Boot:

Utilizând Spring Boot, aplicația beneficiază de funcții precum injectarea dependenței, gestionarea configurației și integrarea ușoară cu bazele de date.

Testare:

Prezența fișierelor de testare (de exemplu, UserRepositoryTests.java) indică faptul că aplicația are teste unitare, care pot fi rulate pentru a asigura funcționalitatea și fiabilitatea caracteristicilor de gestionare a utilizatorilor.

Configurare:

Fișierul application.properties permite configurarea diferitelor setări ale aplicației, cum ar fi conexiunile la baze de date, porturile de server și alte proprietăți specifice mediului.

API:
GET /users
Descriere: Preia și afișează o listă cu toți utilizatorii.
Parametri: niciunul.

GET /users/new
Descriere: Afișează un formular pentru a crea un utilizator nou.
Parametri: niciunul.

POST / users / save

Descriere: salvează un utilizator nou în baza de date.
Parametri: Acceptă un obiect User cu următoarele câmpuri:
{

" email:"string",
"password:" string",
"firstName":"string"
"lastName":"string"
}

GET /users/edit/{id}
Descriere: Afișează un formular pentru a edita un utilizator existent identificat prin ID.
Parametri:
Variabila cale {id}: ID-ul utilizatorului care urmează să fie editat.

GET /users/delete/{id}
Descriere: Șterge un utilizator identificat prin ID.
Parametri:
Variabila cale {id}: ID-ul utilizatorului care urmează să fie șters.