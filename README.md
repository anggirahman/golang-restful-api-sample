
# Golang RestfulAPI sample simple


    mkdir -p $GOPATH/src/github.com/{yours}/restfulapi1

    go get github.com/gorilla/mux

**[GET]** http://localhost:83/people --> Show all data

> [
>     {
>         "id": "1",
>         "firstname": "Anggi",
>         "lastname": "Rahman",
>         "address": {
>             "city": "Bogor",
>             "state": "Indonesia"
>         }
>     },
>     {
>         "id": "2",
>         "firstname": "Ratih",
>         "lastname": "Purnamasari"
>     } ]

**[GET]** http://localhost:83/people/1 --> Show one Data

> {
>     "id": "1",
>     "firstname": "Anggi",
>     "lastname": "Rahman",
>     "address": {
>         "city": "Bogor",
>         "state": "Indonesia"
>     } }

**[POST]** http://localhost:83/people/3 --> Insert Data
    body send =

> {
>     "firstname" : "Arkan",
>     "lastname" : "Sarfaraz"
>}

**[DELETE]** http://localhost:83/people/2 --> Delete data  id = 2
