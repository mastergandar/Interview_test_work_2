
<div align="center">

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api/pin?username=mastergandar&repo=Interview_test_work_2&theme=radical&show_owner=True)

</div>

<div align="center">

![](https://img.shields.io/github/languages/count/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/languages/code-size/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/downloads/mastergndar/Interview_test_work_2/total?style=for-the-badge)
![](https://img.shields.io/github/issues/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/license/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/followers/mastergandar?style=for-the-badge)
![](https://img.shields.io/github/stars/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/commit-activity/m/mastergandar/Interview_test_work_2?style=for-the-badge)
![](https://img.shields.io/github/last-commit/mastergandar/Interview_test_work_2?style=for-the-badge)

</div>

____

<h1 align="center">Описание постановки задачи</h1>
<h2 align="center">Характеристика задачи</h2>

Написать генератор промо кодов и их проверку с помощью Django. Команда должна генерировать коды по выделенным группам, группой может быть номер или строка и сохранять результат в json файл из которого потом можно будет проверить код. Код должен быть уникальным из любого набора символов. Проект должен быть доступен на github с подробной документацией к запуску в README.md.

Например: У нас есть партнеры из агенства недвижимости для которых нужно создать отдельную группу промо кодов по которым они смогут получить плюшки на портале после их ввода.

<h2 align="center">Требование</h2>

Нужно создать комманду которая будет принимать два аргумента amount и group. Результатом выполнения должен стать json файл в котором будут коды сгруппированы по группам. Код должен быть уникальным и не повторяться в остальных уже созданных группах. Json файл не должен перезаписываться, а должен добовлять в существующий файл новые коды и группы.

Для проверки тз нужно написать тест с помощью того же Django который будет тестировать созданную команду. И проверять результирующий файл на соответствие.

После этого нужно написать команду которая будет проверять код в созданом json файле на существование и возвращать ответ.

<h2 align="center">Инструкция</h2>

Для запуска теста нужно выполнить команду ```python manage.py test```.  
Пример вывода:  
```Creating test database for alias 'default'...
System check identified no issues (0 silenced).
setUpTestData: Run once to set up non-modified data for all class methods.
setUp: Run once for every test method to setup clean data.
Json key qwert are equal test key qwert
Json key absad are equal test key absad
Json key group_1 are equal test key group_1
Json promo-code amount=12, group=qwert
Json promo-code amount=19, group=absad
Json promo-code amount=27, group=group_1
Json all promo-code amount=58 and all group count=3
```
Можно изменить тестовый набор данных для генерации Json-файла в переменных ```self.group``` и ```self.count``` функции ```test_custom_command```.
Для проверки на наличие промо-кода в Json-файле введите команду ```manage.py check_promo [промо-код]```.  
Пример вывода для команды ```manage.py check_promo 5d/OXdR1JXLPqIescjrQ6w==```:  
```Promo-code found! Group=absad```

____
| ![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=mastergandar&show_icons=true&theme=radical) | ![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=mastergandar&layout=compact&exclude_repo=Diplom_Py) |
|:----:|:----:|
____

