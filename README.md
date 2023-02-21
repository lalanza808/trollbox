# trollbox

Simple websocket server to allow "trollboxes" in your frontend; real-time chat. Persistence happens in a SQLite database `chat.db`.

`/ws` is the pub/sub websocket endpoint to point clients to.
`/replay` is the http endpoint to replay the chat log so new clients can read scrollback.

You can write your own client, I used `react-use-websocket` in my last site.

## Setup

```
python3 -m venv .venv
.venv/bin/pip install poetry
poetry install
poetry run start
```