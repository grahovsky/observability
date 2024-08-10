для генерации tls:\
chmod +x cert_generation && ./cert_generating 

Запуск\
docker-compose up

если используется se-linux\
chcon -Rt svirt_sandbox_file_t ./certs my.cnf nginx.conf prometheus.yml

интерфейс CMS http://localhost или https://localhost

интерфейс prometheus http://localhost:9000

Скрейперы заведены за nginx, доступны по https по различным locations
