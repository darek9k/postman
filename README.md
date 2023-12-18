Firebase API
Opis
Repozytorium zawiera przykładowe zapytania do Firebase API. Zapytania dotyczą dodawania, edytowania i usuwania osób oraz książek w bazie danych Firebase.
Endpointy
Create person
Metoda: POST
URL: {{url}}/persons.json
Przykładowe zapytanie:

{
    "imie": "Adam",
    "nazwisko": "Ogarek",
    "dataUrodzenia": "1990-02-29T12:00:00",
    "aktywny": true,
    "wzrost": 187.5,
    "zainteresowania": ["siatkówka","gitara"],
    "adres":{
        "kraj":"pl",
        "miasto" : "Gdynia"
    },
    "jezyki":[{"symbol":"pl", "poziom":6},{"symbol":"en", "poziom":4}]
}

Create book
Metoda: POST
URL: {{url}}/books.json
Przykładowe zapytanie:

{
    "tytuł": "Syzyfowe prace",
    "autor": "Sefan Żeromski",
    "liczbaStron": 168,
    "spisTreści": [
        { "nazwaRozdziału":"RozdziaI", "numerStrony": 2 },
        { "nazwaRozdziału":"RozdziaII", "numerStrony": 17 },
        { "nazwaRozdziału":"RozdziaIII", "numerStrony": 31 },
        { "nazwaRozdziału":"RozdziaIV", "numerStrony": 44 },
        { "nazwaRozdziału":"RozdziaV", "numerStrony": 56 }
    ]
}

Get person
Metoda: GET
URL: {{url}}/persons/-NOVGgOEIeL04DJcVKsw.json
Get books
Metoda: GET
URL: {{url}}/books.json
Put book - zmiana autora
Metoda: PUT
URL: {{url}}/books.json
Przykładowe zapytanie:

{
    "tytuł": "Syzyfowe prace",
    "autor": "Sefan Żeromski - kozak",
    "liczbaStron": 168,
    "spisTreści": [
        { "nazwaRozdziału":"RozdziaI", "numerStrony": 2 },
        { "nazwaRozdziału":"RozdziaII", "numerStrony": 17 },
        { "nazwaRozdziału":"RozdziaIII", "numerStrony": 31 },
        { "nazwaRozdziału":"RozdziaIV", "numerStrony": 44 },
        { "nazwaRozdziału":"RozdziaV", "numerStrony": 56 }
    ]
}

Delete book
Metoda: DELETE
URL: {{url}}/books/-NOYNdyo1_QXEOziAHMT.json
