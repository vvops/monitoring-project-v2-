# monitoring-project-v2
Vagrantfile автоматически развернет тестовый стенд мониторинга виртуальной машины.

VAGRANT В ПРОЦЕССЕ НАПИСАНИЯ (НЕ РАБОЧИЙ)
Не решена задача с маштабируемостью prometheus.yml

Описание:
1. Установить на пк Vagrant.
2. Установить установить на пк Virtualbox.
3. Клонируем данный репозиторий с Vagrantfile.
4. Открываем консоль, переходмим в папку с репозиторием.
5. Выполняем команду "Vagrant up" в командной строке.

Результат:
1. Автоматически развернется виртуальная машина.
2. Запустится скрипт на установку Ansible, Node-exporter.
3. Действия будут совершаться через ansible. Установятся следующие программы: Docker, Docker-compose.
4. Запустятся 2 контейнера с prometheus, grafana(уже установлен dashboard 1860).
5. Prometheus будет получать данные с виртуальной машины через node-exporter.
6. Grafana получит в качестве data source данные с prometheus и визуализирует их.
7. Заходим по адресу localhost:3000 на хостовой машине (login - admin ; password - admin)

vagrant: после ограничения доступа пользователей из РФ для загрузки и установки, а также для загрузкии образа машины потребуеться vpn
