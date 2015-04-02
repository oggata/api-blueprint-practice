FORMAT: 1A
HOST: http://example

# Nopaste

タイトルと本文を投稿します


## POST /api/nopaste

+ Request

    + Header

        Host: example

    + Parameters
        + title (required, string) ... タイトル
        + body (required, string) ... 本文

+ Response 201 (text/html)

    + Header

            X-Framework: Ark

    + Body

            {
                "result": {
                    "ok": 1
                }
            }


## GET /api/nopaste/{id}

投稿した記事を閲覧します

+ Request

    + Header

        Host: example

    + Parameters
        + id (required, number) ... ID

+ Response 200 (application/json)

    + Header

            X-Framework: Ark

    + Body

            {
                "result": {
                    "title": "Hello Nopaste",
                    "body": "Text"
                }
            }

## DELETE /api/nopaste/{id}

投稿した記事を削除します

+ Request

    + Header

        Host: example

+ Response 200 (application/json)

    + Header

            X-Framework: Ark

    + Body

            {
                "result": {
                    "ok": 1
                }
            }