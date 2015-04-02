## Endpoints

#### USER API

- **[<code>POST</code> get_user_list](/api_doc/POST_get_user_list.md)**
- **[<code>POST</code> insert_user](/api_doc/POST_insert_user.md)**
- **[<code>POST</code> delete_user](/api_doc/POST_delete_user.md)**
- **[<code>GET</code> get_user_info](/api_doc/GET_get_user_info.md)**


#### How to use mock server

```bash
git clone git@github.com:oggata/api-blueprint-practice.git
cd api-blueprint-practice

npm install -g api-mock
api-mock api_doc/GET_get_user_list_001.md --port 3001
```

#### Test Command

```bash
curl http://localhost:3001/api/get_user_list -X POST
curl http://localhost:3001/api/insert_user -X POST -d "name=taro&profile_comment=test"
curl http://localhost:3001/api/delete_user -X POST -d "user_id=1"
curl http://localhost:3001/api/get_user_info -X GET -d "user_id=1"
```