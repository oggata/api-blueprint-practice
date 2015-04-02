FORMAT: 1A
HOST: http://example

# Nopaste

ユーザーを削除する

## POST /api/delete_user

+ Request

    + Header

        Host: example

    + Parameters
        + user_id (required, number) ... ユーザーID

+ Response 201 (text/html)

    + Header

            X-Framework: Ark

    + Body

            {
                "result": {
                    "ok": 1
                }
            }