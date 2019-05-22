# 2. Редактор объектов

Необходимо описать разработанную в первой работе иерархию классов на языке программирования и реализовать программу с графическим интерфейсом для редактирования свойств объектов.


# 3. Сериализация
В программу, разработанную во второй работе, необходимо добавить возможность сохранения и загрузки списка объектов в файл/из файла.

Необходимо реализовать следующие виды сериализации/десереализации:

бинарная (с использованием готовых библиотечных функций для сериализации);

XML/JSON на выбор (с использованием готовых библиотечных функций для сериализации);

в произвольном текстовом формате (без использования готовых библиотечных функций для сериализации).

Выбор типа сериализации должен выполняться в диалоговом окне сохранения/открытия файла. 

Все сериализаторы должен реализовывать общий интерфейс. Выбор и использование сериализатора следует реализовать таким образом, чтобы добавление нового сериализатора не требовало изменения существующего кода (выбор формата с помощью оператора switch/case делать нельзя).

# 4. Плагины
Необходимо на базе предыдущей работе реализовать минимум 2 плагина для обработки данных перед сохранением в файл.

В зависимости от варианта выбрать тип обработки:

Кодирование в Base64 Base58, Base32, ZBase32.

Архивация.

Шифрование.

Варианты выдаются последовательно в соответствии со списком группы 

При реализации алгоритмов обработки допускается использование сторонних библиотек.

Загрузка плагинов должна производиться автоматически из папки.

При сохранении файла тип обработки (конкретный алгоритм кодирования, архивации, шифрования) должен выбираться из списка, который зависит от загруженных плагинов. 

При открытии файла тип обработки должен выбираться автоматически согласно тому, какая обработка проводилась перед сохранением. Допускается определение типа обработки по расширению файла. Если соответствующий плагин не загружен, вывести сообщение об ошибке.
