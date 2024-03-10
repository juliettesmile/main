# Activities

**1. GET / api/v1/Activities**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities 
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
[
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-14T18:37:31.8333954+00:00",
    "completed": false
  }
]
``` 

**2. POST / api/v1/Activities**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T21:46:47.379Z",
  "completed": true
}
```
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T21:46:47.379Z",
  "completed": true
}
```

**3. POST / api/v1/Activities**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities 
- Заголовки запроса: --H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
```
{
  "id": 000000000,
  "title": "string",
  "dueDate": "2023-06-14T21:46:47.379Z",
  "completed": true
}
```
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-2766172fd5c5144893cc55331317920e-c7c813123e858940-00",
  "errors": {
    "$.id": [
      "Invalid leading zero before '0'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
    ]
  }
}
```

**4. GET /api/v1/Activities/{1}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/1
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 1,
  "title": "Activity 1",
  "dueDate": "2023-06-14T23:03:15.0132375+00:00",
  "completed": false
}
```
**5. GET /api/v1/Activities/{090190190190}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/090190190190 
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-18a8c0fe8f4b23418fe48a61fa5abe8f-14ce21a630a4d44a-00",
  "errors": {
    "id": [
      "The value '090190190190' is not valid."
    ]
  }
}
```

**6. PUT/api /v1 /Activities /{0}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/0 
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T22:07:06.732Z",
  "completed": true
}
```
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T22:07:06.732Z",
  "completed": true
}
```
**7. PUT/api /v1 /Activities /{0}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/777777777777777777777777 
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
```
{
  "id": 777777777777777777777777,
  "title": "string",
  "dueDate": "2023-06-14T22:07:06.732Z",
  "completed": true
}
```
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-611f4757527e5348a563b1709e659403-3b24a25c70daa943-00",
  "errors": {
    "id": [
      "The value '777777777777777777777777' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 27."
    ]
  }
}
```

**8. DELETE /api /v1 /Activities /{1}**

- HTTP-метод: DELETE 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/1 
- Заголовки запроса: -H  "accept: */*"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Wed14 Jun 2023 22:13:40 GMT 
 server: Kestrel 
```

# Authors

**9. GET /api /v1 /Authors**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors 
- Заголовки запроса: -H   "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
  {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  }
```

**10. POST /api /v1 /Authors** 

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d 
- Тело запроса:
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
``` 
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

**11. POST /api /v1 /Authors**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d 
- Тело запроса:
```
{
  "id": 9999999999999,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
``` 
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-34d25312881b7d44b0eb0e05d52a914d-63cb6d270d758740-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```


**12. GET /api /v1 /Authors /authors /books /{101}** 

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/101 
- Заголовки запроса:   -H   "accept: text/plain; v=1.0" 
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
[
  {
    "id": 297,
    "idBook": 101,
    "firstName": "First Name 297",
    "lastName": "Last Name 297"
  }
```

**13. GET /api /v1 /Authors /authors /books /{12345678900000}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/12345678900000 
- Заголовки запроса:   -H   "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4ff3bcbf657807429848d0645daa9da8-eeb816156ca62f48-00",
  "errors": {
    "idBook": [
      "The value '12345678900000' is not valid."
    ]
  }
}
```

**14. GET /api /v1 /Authors /{222}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/222
- Заголовки запроса:   -H   "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 222,
  "idBook": 77,
  "firstName": "First Name 222",
  "lastName": "Last Name 222"
}
```

**15. GET /api /v1 /Authors /{987654321}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/987654321
- Заголовки запроса:   -H   "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-fd64d69e96957d4ba91d49804e4c6ea3-749be28ef40d744a-00"
}
```

**16. PUT /api/v1/Authors/{345}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/345 
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
 {
  "id": 345,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 345,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

**17. PUT /api/v1/Authors/{1234567890000}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/1234567890000
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
 {
  "id": 1234567890000,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b2c959df20376741ae5a4cd3145b2dd8-2226d1454e60ca4c-00",
  "errors": {
    "id": [
      "The value '1234567890000' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```

**18. DELETE /api/v1/Authors/{345}**

- HTTP-метод: DELETE 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/345
- Заголовки запроса:   -H  "accept: */*"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Wed14 Jun 2023 22:36:58 GMT 
 server: Kestrel 
```

# Books

**19. GET/api/v1/Books**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" 
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
{
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-13T22:41:16.431952+00:00"
  }
```

**20. POST /api/v1/Books**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
 {
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:42:27.926Z"
}
```
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:42:27.926Z"
}
```

**21. POST /api/v1/Books**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
 {
  "id": 0101010101,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:42:27.926Z"
}
```
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c349a51117e3a44185868c902c617f79-ae1b796dc1e34149-00",
  "errors": {
    "$.id": [
      "Invalid leading zero before '1'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
    ]
  }
}
```

**22. GET /api/v1/Books/{1}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/Books/1
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа:  200 
- Тело ответа: 
```
{
  "id": 1,
  "title": "Book 1",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 100,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-06-13T22:45:28.4952768+00:00"
}
```

**23. GET /api/v1/Books/{09090909}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/Books/09090909
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-26ea95c7a93d6042ab2a9ee537a6d2a1-a1301ad43fa5284a-00"
}
```

**24. PUT/api/v1/Books/{122}**

- HTTP-метод: PUT 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/Books/122
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d 
- Тело запроса: 
```
{
  "id": 122,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:48:41.731Z"
}
```
- Статус-код ответа:  200 
- Тело ответа: 
```
{
  "id": 122,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:48:41.731Z"
}
```

**25. PUT/api/v1/Books/{11223344556677}**

- HTTP-метод: PUT 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/Books/11223344556677
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса: 
```
{
  "id": 11223344556677,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T22:48:41.731Z"
}
```
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3938009f39a2d442a5da513fe8cc63a2-cb032f733c52264a-00",
  "errors": {
    "id": [
      "The value '11223344556677' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```

**26. DELETE /api/v1/Books/{909}**

- HTTP-метод: DELETE 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/Books/909
- Заголовки запроса:   -H "accept: */*"
- Тело запроса: отсутствует 
- Статус-код ответа:  200 
- Тело ответа: 
```
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Wed14 Jun 2023 22:52:46 GMT 
 server: Kestrel 
```

# CoverPhotos

**27. GET /api/v1/CoverPhotos**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса:   -H "accept: text/plain; v=1.0"
- Тело запроса: отсутствует 
- Статус-код ответа:  200 
- Тело ответа: 
```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  }
```
**28. POST /api/v1/CoverPhotos**

- HTTP-метод: POST 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
{
  "id": 111,
  "idBook": 0,
  "url": "string"
}
``` 
- Статус-код ответа:  200 
- Тело ответа: 
```
{
  "id": 111,
  "idBook": 0,
  "url": "string"
}
```

**29. POST /api/v1/CoverPhotos**

- HTTP-метод: POST 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса:
```
{
  "id": 9988776655,
  "idBook": 0,
  "url": "string"
}
``` 
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-7a5eb22e531ce245979b7336762a3b50-dbabcd3d88766e4f-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```

**30. GET/api/v1/CoverPhotos/books/covers/{78}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/78
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутсвует 
- Статус-код ответа:  200 
- Тело ответа: 
```
[
  {
    "id": 78,
    "idBook": 78,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 78&w=250&h=350"
  }
]
```

**31. GET/api/v1/CoverPhotos/books/covers/{555566667777}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/555566667777
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутсвует 
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-07abd3b1c9dd6b4d961e55db5ac6c715-640b20723ea56a40-00",
  "errors": {
    "idBook": [
      "The value '555566667777' is not valid."
    ]
  }
}
```

**32. GET /api/v1/CoverPhotos/{11}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/11 
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутсвует 
- Статус-код ответа:  200 
- Тело ответа: 
```
{
  "id": 11,
  "idBook": 11,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 11&w=250&h=350"
}
```

**33. GET /api/v1/CoverPhotos/{1111}**

- HTTP-метод: GET 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1111
- Заголовки запроса:   -H  "accept: text/plain; v=1.0"
- Тело запроса: отсутсвует 
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-7b22264dbb5adb43b92b56f11adb13cc-fc6afff0137c1447-00"
}
```

**34. PUT/api/v1/CoverPhotos/{2}**

- HTTP-метод: PUT 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/2 
- Заголовки запроса:   -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d   
- Тело запроса: 
```
{
  "id": 2,
  "idBook": 0,
  "url": "string"
}
```
- Статус-код ответа:  200 
- Тело ответа: 
```
{
  "id": 2,
  "idBook": 0,
  "url": "string"
}
```

**35. PUT/api/v1/CoverPhotos/{111111113333333}**

- HTTP-метод: PUT 
- Полный URL запроса:  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/111111113333333  
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d 
- Тело запроса: 
```
{
  "id": 111111113333333,
  "idBook": 0,
  "url": "string"
}
```
- Статус-код ответа:  400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c22df3de55a5514886f5d43630ca09a5-c7b3b2d7a2696749-00",
  "errors": {
    "id": [
      "The value '111111113333333' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 21."
    ]
  }
}
```

**36. DELETE /api/v1/CoverPhotos/{111}**

- HTTP-метод: DELETE 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/111 
- Заголовки запроса:  -H   "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 
- Тело ответа: 
```
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Wed14 Jun 2023 23:09:20 GMT 
 server: Kestrel 
```

# Users

**37. GET /api/v1/Users**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users 
- Заголовки запроса:  -H   "accept: text/plain; v=1.0"
- Тело запроса: отсутствует
- Статус-код ответа: 200 
- Тело ответа: 
```
  {
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  }
```

**38. POST /api/v1/Users**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
- Заголовки запроса:  -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d   
- Тело запроса: 
```
{
  "id": 22222,
  "userName": "string",
  "password": "string"
}
```
Статус-код ответа: 200 
Тело ответа: 
```
{
  "id": 22222,
  "userName": "string",
  "password": "string"
}
```

**39. POST /api/v1/Users**

- HTTP-метод: POST 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
- Заголовки запроса:  -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d   
- Тело запроса: 
```
{
  "id": 9090909090909,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-ba28e780b246a9419432e6bd055545c4-c5ee6d72f991d74e-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```

**40. GET /api/v1/Users/{5}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/5
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует 
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 5,
  "userName": "User 5",
  "password": "Password5"
}
```

**41. GET /api/v1/Users/{111111}**

- HTTP-метод: GET 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/111111
- Заголовки запроса:  -H   "accept: */*"
- Тело запроса: отсутствует 
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-e113c06961afaa409214e6c758cb050d-b4c5fc66d1e40047-00"
}
```

**42. PUT /api/v1/Users/{90}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/90
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса: 
```
 {
  "id": 90,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 200 
- Тело ответа: 
```
{
  "id": 90,
  "userName": "string",
  "password": "string"
}
```

**43. PUT /api/v1/Users/{909090909090}**

- HTTP-метод: PUT 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/909090909090 
- Заголовки запроса:   -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d
- Тело запроса: 
```
 {
  "id": 909090909090,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 400 
- Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-2e590df3bc20aa4495fdd6d62e503c68-c6b0ca42de436245-00",
  "errors": {
    "id": [
      "The value '909090909090' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 18."
    ]
  }
}
```

**44. DELETE /api/v1/Users/{1}**

- HTTP-метод: DELETE 
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/1
- Заголовки запроса:   -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 
- Тело ответа:  
```
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Wed14 Jun 2023 23:21:48 GMT 
 server: Kestrel 
```
