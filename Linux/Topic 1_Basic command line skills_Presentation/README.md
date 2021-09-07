1. Войти под своим логинам/паролем
2. Создать каталог для упражнений и перейти в него
3. Создать файлы f1 и f2, а также директорию dir1 и в ней файл dir2
4. Скопировать dir1 в dir2 со всеми файлами
5. Удалить dir1
6. Скопировать файл /etc/services в свой каталог
7. Вывести все строки, содержащие HTTP
8. Посчитать количество строчек в нем
9. Исследовать команды more, less, tail, head на файле services
10. Исследовать команды cal, bc
11. Выяснить дату православной пасхи на 2051 год. 

---

2.  ```bash
    root@vagrant:~# mkdir ./HW && cd HW
    ```
3. 
    ```bash
    root@vagrant:~# touch f{1..2} && mkdir dir1 && touch ./dir1/dir2
    ```
4. 
    ```bash
    root@vagrant:~# cp -r dir1 dir2
    ```
5. 
    ```bash
    root@vagrant:~# rm -r dir1
    ```
6. 
    ```bash
    root@vagrant:~# cp /etc/services ~
    ```
7. 
    ```bash
    root@vagrant:~# grep HTTP services
    ```
8. 
    ```bash
    root@vagrant:~# grep -c ^ services
    ```
   
9. 
    ```bash
    root@vagrant:~# more services
    root@vagrant:~# less services
    root@vagrant:~# tail services
    root@vagrant:~# head services
    ```
   
10. 
    ```bash
    root@vagrant:~# cal
    root@vagrant:~# ncal
    root@vagrant:~# bg
    ```
11.
    ```bash
    root@vagrant:~# ncal -o 2051
    05/07/2051
    ```