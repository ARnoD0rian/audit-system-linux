# audit-system-linux
Для запуска программы необходим компилятор MINGW для С++.
Программа состоит из двух файлов: main.cpp и constant.h. Для работы программы из необходимо поместить в одну директорию. Затем необходимо скомпилировать файл main.cpp. Для этого нужно открыть терминал и прописать команду: g++ main.cpp -o auidit. После этого в директории программы появится файл audit. Для запуска программы необходимо открыть терминал и прописать команду: sudo ./audit <pid>. Для того чтобы проводить аудит процесса по его pid. Или: sudo ./audit `pidof <process name>`. Для того чтобы проводить аудит процесса по его имени.
Чтобы отфильтровать логи необходимо открыть терминал и прописать команду: cat ./logger.log | grep “system code”. 
