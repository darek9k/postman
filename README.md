# Firebase API Documentation

## Introduction
This document provides an overview of the Firebase API and describes the available endpoints and their usage.

## Base URL

The base URL for all API requests is `{{url}}`. Please replace `{{url}}` with your Firebase API URL.

## Create Person

### Endpoint
`POST /persons.json`

### Request Body
```json
{
    "imie": "Adam",
    "nazwisko": "Ogarek",
    "dataUrodzenia": "1990-02-29T12:00:00",
    "aktywny": true,
    "wzrost": 187.5,
    "zainteresowania": ["siatkówka", "gitara"],
    "adres": {
        "kraj": "pl",
        "miasto": "Gdynia"
    },
    "jezyki": [
        {"symbol": "pl", "poziom": 6},
        {"symbol": "en", "poziom": 4}
    ]
}
```

### Response
No response is returned for this request.

## Create Book

### Endpoint
`POST /books.json`

### Request Body
```json
{
    "tytuł": "Syzyfowe prace",
    "autor": "Sefan Żeromski",
    "liczbaStron": 168,
    "spisTreści": [
        {
            "nazwaRozdziału": "RozdziaI",
            "numerStrony": 2
        },
        {
            "nazwaRozdziału": "RozdziaII",
            "numerStrony": 17
        },
        {
            "nazwaRozdziału": "RozdziaIII",
            "numerStrony": 31
        },
        {
            "nazwaRozdziału": "RozdziaIV",
            "numerStrony": 44
        },
        {
            "nazwaRozdziału": "RozdziaV",
            "numerStrony": 56
        }
    ]
}
```

### Response
No response is returned for this request.

## Get Person

### Endpoint
`GET /persons/-NOVGgOEIeL04DJcVKsw.json`

### Response
No response is returned for this request.

## Get Books

### Endpoint
`GET /books.json`

### Response
No response is returned for this request.

## Put Book - Change Author

### Endpoint
`PUT /books.json`

### Request Body
```json
{
    "tytuł": "Syzyfowe prace",
    "autor": "Sefan Żeromski - kozak",
    "liczbaStron": 168,
    "spisTreści": [
        {
            "nazwaRozdziału": "RozdziaI",
            "numerStrony": 2
        },
        {
            "nazwaRozdziału": "RozdziaII",
            "numerStrony": 17
        },
        {
            "nazwaRozdziału": "RozdziaIII",
            "numerStrony": 31
        },
        {
            "nazwaRozdziału": "RozdziaIV",
            "numerStrony": 44
        },
        {
            "nazwaRozdziału": "RozdziaV",
            "numerStrony": 56
        }
    ]
}
```

### Response
No response is returned for this request.

## Delete Book

### Endpoint
`DELETE /books/-NOYNdyo1_QXEOziAHMT.json`

### Response
No response is returned for this request.

