# alertmanager-telegram-topic-notification-example

install docker

docker build -t alertmanager-image -f Dockerfile .

docker run -p 127.0.0.1:9093:9093 alertmanager-image

./send_test_alert.sh 

https://gist.github.com/carinadigital/fd2960fdccd77dbdabc849656c43a070