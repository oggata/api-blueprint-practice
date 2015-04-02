FORMAT: 1A
HOST: http://example

# Nopaste

タイトルと本文投稿する１

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