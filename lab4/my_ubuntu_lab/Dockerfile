# Використовуємо офіційний образ Ubuntu з Docker Hub
FROM ubuntu:latest

# Оновлення пакунків та встановлення Apache
RUN apt-get update && \
    apt-get install -y apache2

# Вказуємо ім'я сервера як localhost
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf

# Запуск Apache при старті контейнера
CMD ["apache2ctl", "-D", "FOREGROUND"]

