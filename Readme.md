## 1: Обновляем и устанавливаем необходимые пакеты
Вводим следующие команды:
```
sudo apt update && sudo apt upgrade -y
sudo apt-get install curl
sudo apt update
```
## 2: Устанавливаем Docker и в процессе устновки соглашаемся нажав Y. Также в процессе установки выскочит предупреждение, непугаемся жмем просто Enter - два раза.
```
sudo apt install docker.io
```
## 3: Проверяем версию Docker, должна быть 20.10.12 или выше
```
docker --version
```
## 4: Устанавливаем docker-compose
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
## 5: Устанавливаем права доступа для docker-compose
```
sudo chmod +x /usr/local/bin/docker-compose
```
## 6: Проверяем работу docker-compose должна быть версия 1.29.2 или выше
```
docker-compose --version
```
## 7: Скачиваем и устанавливаем Validator. Соглашаемся, так где надо нажать Y, жмем. Все остальные вопросы, просто жмем Enter на клавиатуре. Когда предложать создать Dashbord, соглашаемся нажав Y, далее придумываем пароль и вводим его в поле терминала. При вводе пароля, его не будет видно. Вводим и жмем Enter на клавиатуре. Все остальное оставляем по умолчанию, нажам на Enter на клавиатуре. Ждем, установка долгая. Если все прошло правильно. терминал выдаст, что надо подключиться через Localhost.
```
curl -O https://raw.githubusercontent.com/shardeum/validator-dashboard/main/installer.sh && chmod +x installer.sh && ./installer.sh
```
