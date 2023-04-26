#  Homework #3. Redis
## Run Redis/Redis Cluster
Развернем Redis в Docker:
![](pic1.png)
Разворачивание RedisCluster:
![](pic2.png)
Если мы не хотим создавать Redis Cluster, настраивая и запуская отдельные экземпляры вручную, как показано выше, существует гораздо более простая система (но мы не узнаем столько же деталей работы). 
```bash
create-cluster start
create-cluster create
```
## Test
Здесь мы подключим наше приложение к базе данных Redis.
![](pic3.png)
Напишем несколько запросов с различными структурами Redis и сравним время их выполнения в Redis и Redis Cluster
В качестве большого JSON файла возьмем датасэт с сайта Kaggle (https://www.kaggle.com/datasets/rmisra/news-category-dataset?resource=download).

Сравним время выполнения различных запросов для Redis и Redis Clsuter
![](pic4.png)
![](pic5.png)
![](pic6.png)
![](pic7.png)
Как можем видеть, где то проигрывает Redis, а где то Redis Cluster.
