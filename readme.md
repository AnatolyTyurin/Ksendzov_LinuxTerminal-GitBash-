## HW_GitBash_1

1) Посмотреть где я - pwd
2) Создать папку – mkdir Ksendzov_git
3) Зайти в папку - cd Ksendzov_git
4) Создать 3 папки - mkdir git1 git2 git3
5) Зайти в любую папку - cd git1
6) Создать 5 файлов (3 txt, 2 json) - touch f1.txt f2.txt f3.txt users.json users2.json
7) Создать 3 папки - mkdir newf_1 newf_2 newf_3
8) Вывести список содержимого папки – ls -la
9) Открыть любой txt файл - vim f1.txt
10) написать туда что-нибудь, любой текст. – «Нажимаем “i” и вводим текст»:
add_in vim_row_1
add_in_vim_row_2
add_in_vim_row_3
11) сохранить и выйти. - “Нажимаем «Esc» и «:wq Enter»”   
12) Выйти из папки на уровень выше - cd ../
13) переместить любые 2 файла, которые вы создали, в любую другую папку. –
cd git1
mv f1.txt ../git2/f1.txt
mv f2.txt ../git2/f2.txt 
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. – 
cp f3.txt ../git3/f3.txt
cp f4.txt ../git3/f4.txt
15) Найти файл по имени – find –name f2.txt
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. - tail -f f1.txt
17) вывести несколько первых строк из текстового файла - head –2 f1.txt
18) вывести несколько последних строк из текстового файла - tail -2 f1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. – less f1.txt
20) вывести дату и время - date
### Задание * 
1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request - 

curl http://162.55.220.72:5006/terminal-hw-request

curl 'http://162.55.220.72:5006/get_method?name=Anatoly&age=35'

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 – 

#!/bin/bash/

cd Ksendzov_git

mkdir git4 git5 git6

cd git4

touch f1.txt f2.txt f3.txt users.json users2.json

mkdir newf_1 newf_2 newf_3

ls -la

cd git4

mv f1.txt ../git5/f1.txt

mv f2.txt ../git5/f2.txt


## HW_GitBash_2
1. Сделать папку dir_1 - mkdir dir_1
2. Зайти в папку dir_1 - cd dir_1
3. Создать папку inner_dir_1 - mkdir inner_dir_1
4. Посмотреть где ты находишься - pwd
5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt - touch tf_1.txt
6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками: - the first 1 - the second 2 - the third 3 – 

cat > tf_2.txt

the first 1

the second 2

the third 3

7. Зайти в папку inner_dir_1 - cd inner_dir_1
8. Через cat сделать текстовый файл tf_3.txt c любыми строками – 

cat > tf_3.txt

doing stuff 1

doing stuff 2

doing stuff_3

“Нажать Ctrl+C”

9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2” –

cat >> tf_3.txt

the second 2

“Нажать Ctrl+C”

10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2” – 

cat >> tf_3.txt

the sec 2

“Нажать Ctrl+C”

11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3” – 

cat >> tf_2.txt

the sec 3

“Нажать Ctrl+C”

12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2” - 

cat >> tf_3.txt

the SeCoNd 2

“Нажать Ctrl+C”

13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2” - 

cat >> tf_2.txt

the seConD 2

“Нажать Ctrl+C”

14. Сделать текстовый файл tf_4.txt в котором будет 15 строк. – 

cat > tf_4.txt

line1

line2

line3

line4

line5

line6

line7

line8

line9

line10

line11

line12

line13

line14

line15

“Нажать Ctrl+C”

Или, например, просто строки с последовательными номерами:

seq 15 | cat > tf_4.txt

15. Сделать текстовый файл tF_5.txt в котором будет 13 строк. – 

line1

line2

line3

line4

line5

line6

line7

line8

line9

line10

line11

line12

line13

“Нажать Ctrl+C”

Или, например, просто строки с последовательными номерами:

seq 15 | cat > tf_4.txt

16. Вывести список всех файлов в папке. – find . -type f
17. Выйти из папки inner_dir_1 – cd ..
18. Вывести содержимое файла tf_3.txt в терминал. - cat inner_dir_1/tf_3.txt
19. Найти путь к файлу tf_4.txt - find $PWD -type f -name tf_4.txt
20. Отчистить файл tf_4.txt от содержимого без удаления самого файла. - > tf_4.txt
21. Найти путь к файлам у которых есть “tf” в названии. - find -type f -name '*tf*'
22. Найти путь к файлам у которых есть “tf” в названии и буквы в любом регистре. - find -type f -iname '*tf*'
23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке – 
grep sec *
24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке - grep -i sec *
25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке – 
grep -w sec *
26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке - grep -iw sec *
27. Найти строки в файлах где есть комбинация букв “second” в текущей папке - grep second *
28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке - grep -i second *
29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем - grep -r second * /
30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке - find $PWD -type f | xargs grep -l second
31. Найти все строки во всех файлах где нет комбинации “second” - grep -nrvw second *
32. Найти только название и путь к файлам где нет комбинации “second” - grep -rlv second *
33. Вывести в терминал 4 последних строк любого текстового файла - tail -n4 tf_2.txt
34. Вывести в терминал 4 первые строки любого текстового файла. - head -n4 tf_4.txt
35. Команда в одну строку. Создать папку и создать текстовый файл с содержимым. – 

mkdir inner_dir_2 && cat > inner_dir_2/newf_1.txt

a

b

c

36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec” - grep -rlw sec | xargs mv -t ../inner_dir_2
37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec” - grep -rlw sec | xargs cp -t inner_dir_1
38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл. – 
grep -rh sec >> newf_2.txt
39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec” - grep -rlw sec | xargs rm
40. Просто вывести в терминал строку “Good job!!” - echo Good job!!
