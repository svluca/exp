# MyMon — v1 Overview

MyMon este un tracker simplu de cheltuieli personale, creat pentru claritate, nu pentru complexitate.

---

Note: MyMon is a working project name. Trademark availability will be checked later, and the name may change to MonMom or another alternative if needed.

---

## Ce este MyMon v1

- Un tool mic pentru urmărirea cheltuielilor personale
- Axat pe claritatea cheltuielilor lunare
- Construit astfel încât să poată crește ulterior
- Nu este o rețea socială (încă)
- Nu este un sistem financiar complet

---

## Public țintă și scop

- Utilizatori inițiali: eu și prieteni apropiați
- Limbă: engleză
- Focus: doar cheltuieli (fără venituri în v1)

---

## Pagini

- Landing Page
  - Vizibilă doar pentru utilizatorii neautentificați
- App / Dashboard
  - Pagina principală după autentificare

---

## Fluxul utilizatorului

- Utilizatorul intră pe site
- Dacă nu este autentificat, vede landing page-ul
- Dacă este autentificat, ajunge direct în dashboard
- Utilizatorul vede:
  - numele sau nickname-ul
  - un mesaj clar:
    - „Luna aceasta ai cheltuit X”
    - sau „Luna trecută ai cheltuit X”
- Apasă butonul „Add expense”
- Completează formularul
- Totalurile și statisticile se actualizează instant

---

## Definirea unei tranzacții (v1)

O tranzacție conține:
- categorie
- sumă
- dată
- comentariu opțional

Reguli de validare:
- suma trebuie să fie mai mare decât 0.01
- suma nu poate fi negativă
- data nu poate fi în viitor
- data poate fi din:
  - luna curentă
  - luna trecută
- comentariul este opțional

---

## Logica lunii

- Lunile sunt calendaristice
- Luna este determinată din data tranzacției (YYYY-MM)
- Nu există logică de „închidere a lunii”
- Nu există joburi automate
- Nu există cicluri salariale personalizate în v1

---

## Categorii

- Listă fixă de categorii
- Include categoria „Other”
- Utilizatorii nu pot crea categorii personalizate în v1

---

## Statistici afișate (v1)

Pentru o lună selectată:
- total cheltuit
- total per categorie (sumă)
- procent per categorie din total
- diagramă vizuală simplă (fără librării externe)

---

## Principii UI / UX

- Text puțin și clar
- Mult spațiu liber
- Overview curat
- Detalii afișate doar la nevoie
- O singură acțiune principală: „Add expense”

---

## Abordare tehnică

- Pornim de la o structură clară
- Construim frontend-ul funcțional mai întâi
- Simulăm backend-ul local
- Backend real și bază de date — mai târziu

---

## Ce NU face parte din v1

- urmărirea veniturilor
- returnări de bani sau împrumuturi
- funcționalități de grup sau prieteni
- categorii personalizate
- cicluri salariale
- exporturi PDF sau rapoarte avansate

---

## Notă finală

Acest proiect pune accent pe claritate, simplitate și învățare.
Complexitatea va fi adăugată doar atunci când aduce valoare reală.
