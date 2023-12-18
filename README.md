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

# Gorest API Documentation

This repository contains the documentation for the Gorest API.

## Endpoints

Below are the available endpoints provided by the Gorest API:

### Get users v1 - szkolenie

```http
GET {{goresturl}}/public/v1/users?page=1&per_page=20&name=A
```

Retrieve a list of users from the v1 API version. You can specify the page number, the number of users per page, and filter by name.

### Get users v2- szkolenie Copy

```http
GET {{goresturl}}/public/v2/users?page=1&per_page=20&active
```

Retrieve a list of users from the v2 API version. You can specify the page number, the number of users per page, and filter by active status.

### Create person

```http
POST {{url}}/persons.json
```

Create a new person with the specified details. The request body should be in JSON format.

### Create book

```http
POST {{url}}/books.json
```

Create a new book with the specified details. The request body should be in JSON format.

### Get books

```http
GET {{url}}/books.json
```

Retrieve a list of books.

### Put book - zmiana autora

```http
PUT {{url}}/books.json
```

Update the author of a book with the specified details. The request body should be in JSON format.

### Delete book

```http
DELETE {{url}}/books/-NOYNdyo1_QXEOziAHMT.json
```

Delete a book with the specified ID.

### Create user - gorest

```http
POST {{goresturl}}/public/v2/users/
```

Create a new user with the specified details. The request body should be in JSON format.

### Create user - gorest Copy

```http
POST {{goresturl}}/public/v2/users/
```

Create a new user with the specified details. The request body should be in JSON format.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


