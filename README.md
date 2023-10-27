# alertmanager-telegram-topic-notification-example

## whrite your telegram credentials in alertmanager.yml
replace <bot_token> <chat_id> <message_id> with your credentials

Install docker to be able to run the next commands
## make image build
```bash
docker build -t alertmanager-image -f Dockerfile .
```
## run image, and connect it to your localhost:9093
```bash
docker run -p 127.0.0.1:9093:9093 alertmanager-image
```
## run script to check if messages sends to the telegram topic
```bash
./send_test_alert.sh 
```
# Info
## send_test_alert.sh taken from: 
https://gist.github.com/carinadigital/fd2960fdccd77dbdabc849656c43a070

## my repo with ansible send to telegram topic feature:
https://github.com/oktend/alertmanager