# Домашнее задание к занятию "Резервное копирование" - `Щербатых А.Е.`

## Задание 1
1. Составьте команду rsync, которая позволяет создавать зеркальную копию домашней директории пользователя в директорию /tmp/backup
2. Необходимо исключить из синхронизации все директории, начинающиеся с точки (скрытые)
3. Необходимо сделать так, чтобы rsync подсчитывал хэш-суммы для всех файлов, даже если их время модификации и размер идентичны в источнике и приемнике.
4. На проверку направить скриншот с командой и результатом ее выполнения

## Выполнение
команда `rsync -a --checksum --verbose --delete --progress --exclude '.*' /home/shcherbatykh/ /tmp/backup`

 ![alt text](https://github.com/Anton-Shcherbatykh/FOPS-32_8/blob/main/screenshots%20%26%20files/%D0%97%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%201_1.jpg)
 ![alt text](https://github.com/Anton-Shcherbatykh/FOPS-32_8/blob/main/screenshots%20%26%20files/%D0%97%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%201_2.jpg)
 ![alt text](https://github.com/Anton-Shcherbatykh/FOPS-32_8/blob/main/screenshots%20%26%20files/%D0%97%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%201_3.jpg)

