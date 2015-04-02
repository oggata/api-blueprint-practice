FORMAT: 1A
HOST: http://example

# Nopaste

ユーザーの情報を取得する

## GET /api/get_user_info

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
                    "user_id": 1,
                    "name": "taro"
                }
            }