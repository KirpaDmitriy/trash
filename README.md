<h1>Передача информации о структурах ОС Linux из ядра к пользователю</h1>

Для загрузки модуля следует выполнить следующие команды: `make; sudo insmod laba.ko`. В ядре появится модуль, который при записи и чтении в файл в директории debugfs будет выводить данные о структуре ядра, соответствующей этому файлу.
Для запуска клиента требуется выполнить: `cd client; gcc app.c`. Получится бинарь с клиентом. Пример использования: `sudo ./a.out 0 1` - вывод данных о структуре `thread_struct`, принадлежащей процессу с PID = 1.
