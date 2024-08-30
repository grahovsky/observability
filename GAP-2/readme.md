для генерации tls:\
chmod +x cert_generation && ./cert_generating 

Запуск\
docker-compose up

если используется se-linux\
chcon -Rt svirt_sandbox_file_t .

- интерфейс CMS http://localhost или https://localhost
- интерфейс prometheus http://localhost:9090

- интерфейс mimir, minio - не выставлен, датасорс, remote_write в конфигах ./configs\
кластер мимир собран по аналогии примера, с адаптацией для предыдущей работы
https://github.com/grafana/mimir/blob/main/docs/sources/mimir/get-started/play-with-grafana-mimir/docker-compose.yml

- интерфейс grafana http://localhost:9000\
добавлены дефолтная доска и доска для проверки relable (site="prod")
