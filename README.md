# Задание B9.5.2
___
Создайте свой docker-image и опубликуйте его в Docker Hub. Можете руководствоваться инструкцией из юнита B9.4.

1) Создайте Dockerfile с нужными настройками.
2) Соберите образ локально.
3) Запустите от него контейнер.
4) Опубликуйте свой докер-образ.

___
docker build -t b952 . 

docker run -p 9911:80 --name server b952

docker tag 19f183e9dcb7 ipleshachev/devops_b9_5_2:latest

docker push ipleshachev/devops_b9_5_2:latest

docker pull ipleshachev/devops_b9_5_2:latest
