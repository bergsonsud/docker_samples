
mysql -u root -p -f datab < dump.sql
mysql -u root -p -f --default-character-set=utf8 datab < dump.sql