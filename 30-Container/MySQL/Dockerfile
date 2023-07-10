# Basisimage
FROM mysql:latest

# Root Passwort
ENV MYSQL_ROOT_PASSWORD modul300lb3

# Datenbank erstellen
ENV MYSQL_DATABASE mydatabase

# Neuer User und Passwort
ENV MYSQL_USER user
ENV MYSQL_PASSWORD modul300lb3

# Named Volume für MySQL
VOLUME /var/lib/mysql

# Port 3306 öffnen
EXPOSE 3306

# MySQL bei Container Boot starten
CMD ["mysqld"]