Алгоритм запуска проекта для выполнения задач в рабочей среде:
1. выполнить docker-compose up для файла docker-compose-pyback.yml
2. запустить c# проект ConsoleClient
При первом запуске генератора с google диска подгружаются веса для нейросети
Изначально решение настроено для отладки на одном хосте, но изменив параметры подключения есть возможность запустить grcp клиент и сервис
на разных машинах.
Адрес grcp сервиса указывается в PyBack/Main.py в функции serve();
Адрес, по которому подключается grcp клиент указывается в файле Program.cs проекта ConsoleClient.cs