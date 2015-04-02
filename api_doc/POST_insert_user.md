FORMAT: 1A
HOST: http://example

# Nopaste

ユーザーを登録し、ユーザーIDを返す


## POST /api/insert_user

+ Request

    + Header

        Host: example

    + Parameters
        + user_name (required, string) ... ユーザー名
        + profile_comment (required, string) ... プロフィール

+ Response 201 (text/html)

    + Header

            X-Framework: Ark

    + Body

            {
                "result": {
                    "user_id": 1
                }
            }
