
# Quick Start
```bash
pip install df-db-connector
```
```bash
docker-compose up -d
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

Contexts are storaged into `json` file. An example of a json file:
```json
{
    "38": {
        "id": 38,
        "labels": {
            "0": [
                "greeting_flow",
                "node1"
            ]
        },
        "requests": {
            "0": "Hi"
        },
        "responses": {
            "0": "Hello, how are you?"
        },
        "misc": {},
        "validation": false,
        "framework_states": {}
    }
}
```