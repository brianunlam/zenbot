Executing ZENBOT

docker-compose up
docker exec -it zenbot_server_1 sh
Load data from binance for 1 day ago
zenbot backfill binance.BTC-USDT --days 1

In order to debug

node --inspect=0.0.0.0 zenbot.js sim binance.BTC-USDT --strategy trend_ema --days 1

