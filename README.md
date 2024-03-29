# MobileDevColt

_Автор: @coltmister Мобильная разработка_
| Соцсеть | Данные |
|:---------:|:-----------------------:|
| VK | vk.com/kotkeks1 |
| TG | coltadmin |
| Email | colt.mister@gmail.com |

## Лабораторная 1

Для запуска данной программы необходим лишь Python, никаких внешних зависимостей нет.
Запуск проводится командой `python main.py`

Содержание папки:

```
data.csv - файл с исходными данными
result.txt - файл с выводом результата
main.py - файл с исходным кодом
```

Выполнялся 10 вариант. Программа, в принципе, сделана универсальной под несколько вариантов:

- [x] Возможность указывать стоимость как для первых, так и для последующих **исходящих**
- [x] Возможность указывать стоимость как для первых, так и для последующих **входящих**
- [x] Возможность указывать стоимость как для первых, так и для последующих **смс**

Также были проведены тесты на скорость работы программы:

1. На примере с диска: **-> 0 секунд**
2. На 1000 записей: **0.00398 секунд**
3. На 10 000 записей: **0.04092 секунд**
4. На 100 000 записей: **0.38166 секунд**
5. На ~1 000 000 записей: **1.96120 секунд**

В следующей версии 2.0 :

- [ ] Добавить тарификацию по времени

## Лабораторная 2

Для запуска данной программы необходим Python, а также 2 внешних библиотеки.
Установить эти библиотеки можно командами
`pip install numpy`
`pip install plotly`
Запуск проводится командой `python main.py`
При выполнении открывается окно браузера с выводом графика зависимости объема трафика от времени.
Пример графика приведен в файле `plot.png`

Содержание папки:

```
dump.json - файл с исходными данными
result.txt - файл с выводом результата
main.py - файл с исходным кодом
plot.png - файл с примером графика
```

Выполнялся 10 вариант.
Также были проведены тесты на скорость работы программы:

1. На примере с диска с отображением графика: **1 секунда**
2. На примере с диска без отображения графика: **0.07 секунд**

При условии того, что использовался json файл.

## Лабораторная 3

Небольшая вводная:
По факту, формирование документа - это отдельный модуль, который можно использоват в удобном веб-интерфейсе, например в связке Python-фреймворка Django и любого Фронтэнда.
В целом тарификация - достаточно большой пласт, который лучше всего формировать при наличии полного понимания тонкостей системы, как например с округлением трафика\звонков. Плюс, мы не можем знать и других тонкостей, например, что именно будет удобно конечному пользователю.

---

Для запуска данной программы необходим Python, а также 2 внешних библиотеки.
Установить эти библиотеки можно командами
`pip install docxtpl`
`pip install docx2pdf`
Запуск проводится командой `python main.py`
При выполнении генерируются два файла
`{Название}.docx`
`{Название}.pdf`
Примеры генерации приведены в файлах
`Счет №1337.docx`
`Счет №1337.pdf`

Содержание папки:

```
dump.json - файл с исходными данными для интернет
data.csv - файл с исходными данными для мобильной связи
main.py - файл с исходным кодом
Счет №1337.docx - файл-счет в формате Word
Счет №1337.pdf - файл-счет в формате PDF
```

Выполнялся 10 вариант.
Также были проведены тесты на скорость работы программы(при условии, что пользователь вводит прописную сумму моментально):

1. На примерах данных без учета генерации PDF: **0.16 секунд**
2. На примерах данных c учета генерации PDF: **4.27 секунды**
