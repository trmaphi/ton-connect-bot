# ton-connect-bot
A simple bot written on Python to interact with TON wallets using Ton Connect protocol

The running public instance can be found at https://t.me/test_tonconnect_bot

## How to launch

### Redis
If you want to use permanent TON Connect storage you should [set up Redis](https://redis.io/docs/getting-started/) or any other database.

```
docker compose up -d
```

### Install dependencies:

```bash
uv sync
```

### Set up `.env`:

```dotenv
TOKEN='1111:ABCD'  # your bot token here
MANIFEST_URL='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json'
```

### Run bot

```python
python src/main.py
```
