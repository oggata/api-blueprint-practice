FORMAT: 1A
HOST: http://example

# Nopaste

登録されたユーザーの一覧を返す


## POST /api/get_user_list

+ Request

    + Header

        Host: example

    + Parameters

+ Response 201 (text/html)

    + Header

            X-Framework: Ark

    + Body

            {
                "result" : {
                    "next_page":2,
                    "previous_page":null,
                    "total_entries":40,
                    "last_page":4,
                    "first_page":1,
                    "current_page":1,
                    "list":[
                        { 
                            "user_id":1,
                            "name":"taro"
                        },
                        { 
                            "user_id":2,
                            "name":"jiro"
                        },
                        { 
                            "user_id":3,
                            "name":"hanako"
                        }
                    ]
                }
            }












