### Terminal 
<div> 
  <img src="https://github.com/devicons/devicon/blob/master/icons/linux/linux-original.svg" title="Linux" **alt="Linux" width="40" height="40"/> 
</div>

### HW_1

1) Посмотреть где я
```
pwd
```
2) Создать папку
```
mkdir foldername
```
3) Зайти в папку
```
cd foldername
```
4) Создать 3 папки
```
mkdir foldername_1
mkdir foldername_2
mkdir foldername_3
```
5) Зайти в любоую папку
```
cd foldername_2
```
6) Создать 5 файлов (3 txt, 2 json)
```
touch filename_1.txt
touch filename_2.txt
touch filename_3.txt
touch filename_4.json
touch filename_5.json
```
7) Создать 3 папки
```
mkdir foldername_1.1
mkdir foldername_2.1
mkdir foldername_3.1
```
8) Вывести список содержимого папки
```
ls -la foldername_1.1
или
ls -l foldername_1.1
```
9) Открыть любой txt файл
```
cat filename_3.txt
vim filename_3.txt
```
10) написать туда что-нибудь, любой текст.
```
insert
"любой текст"
```
11) + сохранить и выйти.
```
esc : wq
```
12) Выйти из папки на уровень выше
```
cd ..
```
13) переместить любые 2 файла, которые вы создали, в любую другую папку.
```
mv foldername_2/filename_1.txt foldername_1.1/filename_1.txt
mv foldername_2/filename_4.json foldername_3.1/filename_4.json
```
14) скопировать любые 2 файла, которые вы создали, в любую другую папку.
```
cp foldername_2/filename_1.txt foldername_1.1/filename_1.txt
cp foldername_2/filename_4.json foldername_3.1/filename_4.json
```
15) Найти файл по имени
```
find foldername -name filename_3.txt
```
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.
```
grep line filename_3.txt
```
17) вывести несколько первых строк из текстового файла
```
head filename_3.txt
```
18) вывести несколько последних строк из текстового файла
```
tail filename_3.txt
```
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
```
less filename_3.txt
```
20) вывести дату и время
```
date
```
Задание *
1) Отправить http запрос на сервер --
```
curl http://162.55.220.72:5005/terminal-hw-request
curl "http://162.55.220.72:5005/get_method?name=Pavel&age=24"
```
2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
```
#!/bin/bash

echo "Зайти в папку"
cd foldername

echo "Создать 3 папки"
mkdir foldername_1 foldername_2 foldername_3

echo "Зайти в любоую папку"
cd foldername_2

echo "Создать 5 файлов (3 txt, 2 json)"
touch filename_1.txt filename_2.txt filename_3.txt filename_4.json filename_5.json 

echo "Создать 3 папки"
mkdir foldername_1.1 foldername_2.1 foldername_3.1

echo "Вывести список содержимого папки"
ls -la

echo "переместить любые 2 файла в другую папку"
mv foldername_2/filename_1.txt foldername_1.1/filename_1.txt foldername_new
```
___
### HW_2
1. Сделать папку dir_1 
```
   mkdir dir_1
```
2. Зайти в папку dir_1
```
   cd dir_1
```
3. Создать папку inner_dir_1 
  ```
  mkdir inner_dir_1
```
4. Посмотреть где ты находишься
 ```
   pwd
```
5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt
 ```
   touch tf_1.txt
```
6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:

- the first 1

- the second 2

- the third 3
```
cat > tf_2.txt 
  - the first 1
  - the second 2
  - the third
  Ctrl + D
```  
7. Зайти в папку inner_dir_1
```
cd inner_dir_1
```
8. Через cat сделать текстовый файл tf_3.txt  c любыми строками  
 ```
 cat > tf_3.txt  
 ввести текст
 Ctrl + D
 ```
9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2” 
 ```  
cat >> tf_3.txt
the second 2
Ctrl + D
```
10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”  
```   
cat >> tf_3.txt 
the sec 2
Ctrl + D
```
11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”
```   
cat >> tf_2.txt
the sec 3
Ctrl + D
```
12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2” --> 
```   
cat >> tf_3.txt
the SeCoNd 2
Ctrl + D
```
13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2” 
```   
cat >> tf_2.txt
the seConD 2
Ctrl + D
```
14. Сделать текстовый файл tf_4.txt в котором будет 15 строк 
```   
cat > tf_4.txt
ввести текст
Ctrl + D
```
15. Сделать текстовый файл tF_5.txt в котором будет 13 строк
```   
cat > tf_5.txt 
ввести текст
Ctrl + D
```
16. Вывести список всех файлов в папке
```
ls -la
```
17. Выйти из папки inner_dir_1
```
cd ../
```
18. Вывести содержимое файла tf_3.txt в терминал
```
cat tf_3.txt
```
19. Найти путь к файлу tf_4.txt
```
find -name tf_4.txt
```
20. Очистить файл tf_4.txt от содержимого без удаления самого файла
```
inner_dir_1/tf_4.txt
```
21. Найти путь к файлам у которых есть  “tf” в названии
```
find -type f -name "*tf*"
```
22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре
```
find -type f -iname "*tf*"
```
23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке
```
grep sec *
```
24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке
```   
grep -i sec *
```
25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
```
grep -w sec *
```
26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке
```
grep -iw sec *
```
27. Найти строки в файлах где есть комбинация букв “second” в текущей папке
```
grep second *
```
28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке
```
grep -i second *
```
29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем
```
grep -r second
```
30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке
```
grep -l second * | xargs realpath
```
31. Найти все строки во всех файлах где нет комбинации “second”
```
grep -r -v second
```
32. Найти только название и путь к файлам где нет комбинации “second”
```
grep -r -l -v second *
```
33. Вывести в терминал 4 последних строк любого текстового файла
```
tail -4 tf_2.txt
```
34. Вывести в терминал 4 первые строки любого текстового файла.
```
head -4 tf_2.txt
```
35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.
```
mkdir inner_dir_2 && cat >> inner_dir_2/tf_6.txt
```
36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
```
grep -r -l -w sec | xargs mv -t inner_dir_2
```
37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
```
grep -r -l -w sec | xargs cp -t inner_dir_1
```
38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
```
grep -r -h sec >> new.txt
```
39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
```
grep -r -l -w sec | xargs rm
```
40. Просто вывести в терминал строку “Good job!!”
```  
echo 'Good job !!'
```
