
# Quick Start
## Requirements
```bash
pip install -r requirements.txt
```

Run the the code.
```bash
python main.py
```

Interact with the script:
```
type your answer: Hi
2022-04-27 17:41:20,560-           root: 60:        turn_handler():INFO - in_request=Hi -> Hello, how are you?
type your answer:
```

Contexts are storaged into postgresdb. You can use `psql` with password `pass` to connect to the db and check context:
```psql
psql  --dbname=test -U postgres --host=localhost  --port=5432
Password:
test=# select * from contexts;
 id |                                                                                       context                                                                                        
----+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 97 | {"id": 97, "labels": {"0": ["greeting_flow", "node1"]}, "requests": {"0": "Hi"}, "responses": {"0": "Hello, how are you?"}, "misc": {}, "validation": false, "framework_states": {}}
(1 row)
```