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
Задание * 1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request - 
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

