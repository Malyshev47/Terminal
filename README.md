# Terminal

# HW_1

 1. Посмотреть, где я
 
	`pwd`

 2. Создать папку
 
	`mkdir hw1`

 3. Зайти в папку
 
	`cd hw1`

 4. Создать 3 папки
 
	`mkdir zz1 zz2 zz3`

 5. Зайти в любую папку
 
	`cd zz1`

 6. Создать 5 файлов (3 txt, 2 json)
 
	`touch ff.txt ff1.txt ff2.txt js.json js1.json`

 7. Создать 3 папки	
 
	`mkdir zz4 zz5 zz6`

 8. Вывести список содержимого папки
 
	`ls -la`

 9. Открыть любой txt файл
 
	`start ff.txt или vim ff.txt`

 10. Написать туда что-нибудь, любой текст
 
	vim ff.txt
 	Внутри vim нажать INSERT и ввести строки 123 и ggg далее нажать ESCAPE

 11. Сохранить и выйти
 
	Ввести внизу :wq

 12. Выйти из папки на уровень выше
 
	cd ../

 13. Переместить любые 2 файла, которые вы создали, в любую другую папку
 
	mv zz1/ff.txt zz2/ff.txt
 	mv zz1/ff1.txt zz2/ff1.txt
 	или
 	mv {file.jpg,file1.jpg} "C:\Users\hw1\zz1"

 14. Скопировать любые 2 файла, которые вы создали, в любую другую папку
 
	cp zz1/ff2.txt zz3/ff2.txt
 	cp zz1/js.json zz3/js.json
 	или
 	cp file.jpg file1.jpg zz1/ (если находитесь в директории где есть копируемые файлы и директория куда вы их копируете)
 	или
 	cp {file.jpg,file1.jpg} "C:\Users\hw1\zz1"

 15. Найти файл по имени
 
	find . -name ff.txt

 16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает
 
	tail -f gg.txt
 	tail -f gg.txt | grep 4 gg.txt
 	(в режиме реального времени строки с 4)

 17. Вывести несколько первых строк из текстового файла	
 
	head -2 gg.txt

 18. Вывести несколько последних строк из текстового файла
 
	tail -2 gg.txt

 19. Просмотреть содержимое длинного файла (команда less) изучите как она работает
 
	less gg.txt
	Перемещение по строкам с помощью кнопок J и K “/line” пример поиска по файлу перемещение вниз по «подсвеченным» строкам (словам) – N, вверх – SHIFT+N
	Перемещение сразу по странице – F и B
	Выход - q

 20. Вывести дату и время
 
	date
  
  
 # HW_2
 
 1. Сделать папку dir_1
 
	`mkdir dir_1`

 2. Зайти в папку dir_1
 
	`cd dir_1`

 3. Создать папку inner_dir_1
 
	`mkdir inner_dir_1`

 4. Посмотреть где ты находишься
 
	`pwd`

 5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt
 
	`touch tf_1.txt`

 6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками: the first 1, the second 2, the third 3
 
 `cat >> tf_2.txt
  the first 1
	the second 2
	the third 3`

 7. Зайти в папку inner_dir_1
 
	`cd inner_dir_1`

 8. Через cat сделать текстовый файл tf_3.txt  c любыми строками
 
	`cat >> tf_3.txt
  True
	False
	Pixel`

 9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”
 
	`cat >> tf_3.txt
	the second 2`

 10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”
 
	cat >> tf_3.txt
	the sec 2

 11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”
 
	cat >> tf_2.txt
	the sec 3

 12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”
 
	cat >> tf_3.txt
	the SeCoNd 2

 13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”
 
	cat >> tf_2.txt
	the seConD 2

 14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.
 
	cat >> tf_4.txt
	1
	2
	3
	4
	5
	6
	7
	8
	9
	10
	11
	12
	13
	14
	15

 15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.
 
	cat >> tf_4.txt
	1
	2
	3
	4
	5
	6
	7
	8
	9
	10
	11
	12
	13

 16. Вывести список всех файлов в папке.
 
	ls -la

 17. Выйти из папки inner_dir_1
 
	cd ..

 18. Вывести содержимое файла tf_3.txt в терминал.
 
	cat inner_dir_1/tf_3.txt

 19. Найти путь к файлу tf_4.txt
 
	find . -name "tf_4*"
	./inner_dir_1/tf_4.txt

 20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.
 
	: > ./inner_dir_1/tf_4.txt

 21. Найти путь к файлам у которых есть  “tf” в названии.
 
	find . -name "tf*"
	./inner_dir_1/tf_2.txt
	./inner_dir_1/tf_3.txt
	./inner_dir_1/tf_4.txt
	./tf_1.txt
	./tf_2.txt

 22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.
 
	find . -iname "tf*"
	./inner_dir_1/tf_2.txt
	./inner_dir_1/tf_3.txt
	./inner_dir_1/tf_4.txt
	./inner_dir_1/tF_5.txt
	./tf_1.txt
	./tf_2.txt

 23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке
 
	grep "sec" ./*
	grep: ./inner_dir_1: Is a directory
	./tf_2.txt:the second 2

 24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке
 
	grep -i "sec" ./*
	grep: ./inner_dir_1: Is a directory
	./tf_1.txt:SeCond
	./tf_2.txt:the second 2

 25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
 
	grep -w "sec" ./*

 26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке
 
	grep -w -i "sec" ./*

 27. Найти строки в файлах где есть комбинация букв “second” в текущей папке
 
	grep "second" ./*
	grep: ./inner_dir_1: Is a directory
	./tf_2.txt:the second 2

 28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке
 
	grep -i "second" ./*
	grep: ./inner_dir_1: Is a directory
	./tf_1.txt:SeCond
	./tf_2.txt:the second 2

 29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем
 
	grep -r "second" ./*
	./inner_dir_1/tf_3.txt:the second 2
	./tf_2.txt:the second 2

 30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке
 
	grep -l "second" ./*
	grep: ./inner_dir_1: Is a directory
	./tf_2.txt

 31. Найти все строки во всех файлах где нет комбинации “second”
 
	grep -v -r "second" ./*
	./inner_dir_1/tf_2.txt:the sec 3
	./inner_dir_1/tf_2.txt:the seConD 2
	./inner_dir_1/tf_3.txt:True
	./inner_dir_1/tf_3.txt:False
	./inner_dir_1/tf_3.txt:Pixel
	./inner_dir_1/tf_3.txt:the sec 2
	./inner_dir_1/tf_3.txt:the SeCoNd 2
	./inner_dir_1/tf_4.txt:sEC
	./inner_dir_1/tF_5.txt:1
	./inner_dir_1/tF_5.txt:2
	./inner_dir_1/tF_5.txt:3
	./inner_dir_1/tF_5.txt:4
	./inner_dir_1/tF_5.txt:5
	./inner_dir_1/tF_5.txt:6
	./inner_dir_1/tF_5.txt:7
	./inner_dir_1/tF_5.txt:8
	./inner_dir_1/tF_5.txt:9
	./inner_dir_1/tF_5.txt:10
	./inner_dir_1/tF_5.txt:11
	./inner_dir_1/tF_5.txt:12
	./inner_dir_1/tF_5.txt:13
	./tf_1.txt:SeCond
	./tf_2.txt:the first 1
	./tf_2.txt:the third 3

 32. Найти только название и путь к файлам где нет комбинации “second”
 
	grep -v -r -l "second" ./*
	./inner_dir_1/tf_2.txt
	./inner_dir_1/tf_3.txt
	./inner_dir_1/tf_4.txt
	./inner_dir_1/tF_5.txt
	./tf_1.txt
	./tf_2.txt

 33. Вывести в терминал 4 последних строк любого текстового файла
 
	tail -n 4 ./inner_dir_1/tf_3.txt
	Pixel
	the second 2
	the sec 2
	the SeCoNd 2

 34. Вывести в терминал 4 первые строки любого текстового файла.
 
	head -n 4 ./inner_dir_1/tf_3.txt
	True
	False
	Pixel
	the second 2

 35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.
 
	mkdir folder_1 && echo "file" > file_1.txt

 36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
 
	grep -lr sec | xargs mv -t ./folder_1

 37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
 
	grep -lr sec | xargs cp -t ./folder_1

 38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
 
	grep -hr sec >> output.txt

 39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
 
	grep -lr sec | xargs rm

 40. Просто вывести в терминал строку “Good job!!”
 
	echo 'Good job!!'
