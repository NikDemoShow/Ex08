
# Ex07 Разработка класса MyString

### Задача №1

> Разработать класс MyString (строка). 

Хранение символов осуществляется в динамическом массиве.

- **MyString( const char* )** - конструктор с одним параметром (есть значение по-умолчанию **nullptr**).
- **MyString( std::string )** - конструктор с одним параметром.
- **MyString( const MyString& )** - конструктор копирования.
- **MyString( MyString&& )** -  конструктор переноса.
- **~MyString()** - деструктор.
- **length()** - количество символов (длина строки).
- **get()** - возвращение указателя на данные (тип `char*`).

> Реализовать в классе MyString перегрузку операций:

- **operator+** - сложение (конкатенация двух строк).
- **operator-** - вычитание (из первой строки удаляются все символы, присутствующие во второй строке).
- **operator\*** - умножение на целое число (строка повторяется заданное число раз).
- **operator=** - копирующее присваивание.
- **operator=** - перемещающее присваивание.
- **operator==** - сравнение на равенство.
- **operator!=** - сравнение на неравенство.
- **operator>** - лексографическое сравнение .
- **operator<** - лексографическое сравнение. 
- **operator>=** - лексографическое сравнение. 
- **operator<=** - лексографическое сравнение. 
- **operator!** - у латинских букв меняется регистр.
- **operator[]** - доступ к символу по индексу.
- **operator()** - поиск подстроки.
- **operator>>** - чтение из потока.
- **operator>>** - запись в поток.

*Примечание*

Класс и методы можно использовать следующим образом:

```cpp
#include "MyString.h"

int main()
{
    MyString s1("Hello,");
    MyString s2("world!");
    MyString s3;
    s3 = s1 + s2;
    std::cout << s3;
    std::cout << s3("ll");   // 2
    std::cout << s3("mama"); // -1
}
```

### Задача №2

> Написать демонстрационную программу с использованием класса Fraction

### Задача №3

> Необходимо оформить код в соответствии со стандартом, описанном в https://google.github.io/styleguide/cppguide.html 
 
При нарушении стандартов оформления, код не пройдет проверку программой **cpplint**. Узнать замечания можно в разделе **Checks->cpplint**.


## Структура проекта

- **MyString.h** - заголовочный файл для класса **MyString**.
- **MyString.cpp** - файл с реализацией методов класса **MyString**.
- **main.cpp** - домонстрационная программы для работы с классом **MyString**.

Файл `MyString.h` помещаются в каталог `include`
Файлы `MyString.cpp, main.cpp` помещаются в каталог `src` 
 
## Список участников/веток

1. Бакурский    Андрей  Сергеевич   19 ПИ-1 b1
1. Балаян   Роман   Каренович   19 ПИ-1 b2
1. Бекина   Светлана    Сергеевна   19 ПИ-2 b3
1. Боряев   Сергей  Сергеевич   19 ПИ-1 b4
1. Бурцев   Роман   Андреевич   19 ПИ-1 b5
1. Варгин   Дмитрий Александрович   19 ПИ-1 b6
1. Вотинова Ксения  Константиновна  19 ПИ-1 b7
1. Герасимов    Алексей Александрович   19 ПИ-1 b8
1. Грачев   Александр   Евгеньевич  19 ПИ-1 b9
1. Долгополов   Алексей Геннадьевич 19 ПИ-1 b10
1. Думаревская  Татьяна Николаевна  19 ПИ-2 b11
1. Емшанов  Павел   Андреевич   19 ПИ-1 b12
1. Игумнова Наталья Дмитриевна  19 ПИ-2 b13
1. Климов   Алексей Сергеевич   19 ПИ-1 b14
1. Лукичева Полина  Александровна   19 ПИ-1 b15
1. Лупехина Людмила Евгеньевна  19 ПИ-1 b16
1. Макаров  Вадим   Дмитриевич  19 ПИ-1 b17
1. Мурзинов Михаил  Денисович   19 ПИ-1 b18
1. Николаева    Олеся   Игоревна    19 ПИ-1 b19
1. Османов  Ислам   Рамилевич   19 ПИ-1 b20
1. Павлова  Дарья   Андреевна   19 ПИ-1 b21
1. Сапожников   Андрей  Михайлович  19 ПИ-1 b22
1. Сафронов Иван    Дмитриевич  19 ПИ-1 b23
1. Смирнов  Григорий    Андреевич   19 ПИ-1 b24
1. Стоянов  Станислав   Степанович  19 ПИ-1 b25
1. Трухин   Егор    Сергеевич   19 ПИ-1 b26
1. Ускова   Елена   Максимовна  19 ПИ-1 b27
1. Успенский    Владимир    Иванович    19 ПИ-1 b28
1. Хорошилова   Марина  Александровна   19 ПИ-1 b29
1. Баранов  Илья    Андреевич   19 ПИ-2 b30
1. Бекусов  Михаил  Александрович   19 ПИ-2 b31
1. Бодров   Егор    Алексеевич  19 ПИ-2 b32
1. Бредихин Максим  Владимирович    19 ПИ-2 b33
1. Даняев   Артем   Андреевич   19 ПИ-2 b34
1. Дыряев   Даниил  Александрович   19 ПИ-2 b35
1. Зиганшин Никита  Русланович  19 ПИ-2 b36
1. Конина   Татьяна Дмитриевна  19 ПИ-2 b37
1. Костин   Андрей  Олегович    19 ПИ-2 b38
1. Мингбоев Худайберди  Абдухаким угли  19 ПИ-2 b39
1. Моисеев  Роман   Михайлович  19 ПИ-2 b40
1. Моничева Арина   Александровна   19 ПИ-1 b41
1. Мушка    Никита  Андреевич   19 ПИ-2 b42
1. Николаев Иван    Александрович   19 ПИ-2 b43
1. Ожиганова    Полина  Максимовна  19 ПИ-2 b44
1. Рыжова   Ирина   Игоревна    19 ПИ-2 b45
1. Салахов  Рамазан Маратович   19 ПИ-2 b46
1. Семаев   Никита  Юрьевич 19 ПИ-2 b47
1. Скугаревский Александр   Сергеевич   19 ПИ-2 b48
1. Столбов  Ярослав Владиславович   19 ПИ-2 b49
1. Таценко  Алексей Михайлович  19 ПИ-1 b50
1. Таценко  Илья    Михайлович  19 ПИ-1 b51
1. Тюлин    Игорь   Викторович  19 ПИ-2 b52
1. Фатин    Максим  Романович   19 ПИ-2 b53
1. Хорошавина   Екатерина   Андреевна   19 ПИ-2 b54
1. Цветков  Дмитрий Алексеевич  19 ПИ-2 b55
1. Шарунов  Евгений Александрович   19 ПИ-2 b56
1. Шатилов  Виктор  Алексеевич  19 ПИ-2 b57
1. Широков  Александр   Анатольевич 19 ПИ-2 b58
1. Стифеев  Никита  Андреевич   19 ПИ-2 b59
1. Малинин  Дмитрий Дмитриевич  19 ПМИ-2 b60
1. Бакланов Алексей Александрович   19 ПМИ-2 b61
1. Баринов  Даниил  Сергеевич   19 ПМИ-1 b62
1. Богомазов    Михаил  Васильевич  19 ПМИ-1 b63
1. Бугров   Лев Валерьевич  19 ПМИ-1 b64
1. Бузанов  Егор    Андреевич   19 ПМИ-1 b65
1. Варлачёв Валерий Максимович  19 ПМИ-1 b66
1. Голованов    Денис   Максимович  19 ПМИ-1 b67
1. Дробот   Елизавета   Денисовна   19 ПМИ-1 b68
1. Жаравина Полина  Дмитриевна  19 ПМИ-1 b69
1. Зайцев   Тимур   Олегович    19 ПМИ-1 b70
1. Кабанов  Денис   Сергеевич   19 ПМИ-1 b71
1. Канев    Владислав   Олегович    19 ПМИ-1 b72
1. Карцева  Мария   Дмитриевна  19 ПМИ-1 b73
1. Касьянов Никита  Юрьевич 19 ПМИ-1 b74
1. Козлова  Дарья   Андреевна   19 ПМИ-1 b75
1. Кузнецов Михаил  Дмитриевич  19 ПМИ-1 b76
1. Лавров   Артём   Романович   19 ПМИ-1 b77
1. Матвеев  Андрей  Сергеевич   19 ПМИ-1 b78
1. Машанова Карина  Алексеевна  19 ПМИ-1 b79
1. Наумов   Никита  Александрович   19 ПМИ-1 b80
1. Нещеткин Глеб    Максимович  19 ПМИ-1 b81
1. Пасманик Ирина   Дмитриевна  19 ПМИ-1 b82
1. Рогозян  Анастасия   Тимофеевна  19 ПМИ-1 b83
1. Соболев  Данил   Александрович   19 ПМИ-1 b84
1. Софронов Валерий Александрович   19 ПМИ-1 b85
1. Трутнев  Алексей Игоревич    19 ПМИ-1 b86
1. Тумаков  Вадим   Сергеевич   19 ПМИ-1 b87
1. Фролова  Ольга   Михайловна  19 ПМИ-1 b88
1. Шарибжанова  Диана   Рашидовна   19 ПМИ-1 b89
1. Щеникова Анна    Юрьевна 19 ПМИ-1 b90
1. Андросов Вадим   Дмитриевич  19 ПМИ-2 b91
1. Бирина   Елизавета   Сергеевна   19 ПМИ-2 b92
1. Булатов  Дмитрий Александрович   19 ПМИ-2 b93
1. Демашов  Никита  Александрович   19 ПМИ-2 b94
1. Добряев  Иван    Александрович   19 ПМИ-2 b95
1. Дрожжачих    Евгений Валерьевич  19 ПМИ-2 b96
1. Егорова  Кристина    Олеговна    19 ПМИ-2 b97
1. Загоскин Владислав   Андреевич   19 ПМИ-2 b98
1. Зарубина Ирина   Михайловна  19 ПМИ-2 b99
1. Иванов   Даниил  Андреевич   19 ПМИ-2 b100
1. Клыков   Антон   Романович   19 ПМИ-2 b101
1. Королев  Денис   Витальевич  19 ПМИ-2 b102
1. Краюшкина    Екатерина   Алексеевна  19 ПМИ-2 b103
1. Назаров  Вячеслав    Андреевич   19 ПМИ-2 b104
1. Оленев   Дмитрий Сергеевич   19 ПМИ-2 b105
1. Панина   Полина  Сергеевна   19 ПМИ-2 b106
1. Прыгаев  Денис   Алексеевич  19 ПМИ-2 b107
1. Рогов    Андрей  Дмитриевич  19 ПМИ-2 b108
1. Симонова Арина   Валерьевна  19 ПМИ-2 b109
1. Созинов  Кирилл  Игоревич    19 ПМИ-2 b110
1. Титова   Нина    Ивановна    19 ПМИ-2 b111
1. Уртюков  Илья    Алексеевич  19 ПМИ-2 b112
1. Хорев    Егор    Алексеевич  19 ПМИ-2 b113
1. Шабаршин Леонид  Георгиевич  19 ПМИ-2 b114


## Алгоритм выполнения работы

Для выполнения работы необходимо:

1. Выполнить *fork* репозитария в свой аккаунт.
1. Выполнить клонирование репозитария из своего аккаунта к себе на локальную машину (`git clone`).
1. Создать ветку **git** с индивидуальным номером (`git branch имя_ветки`).
1. Сделать ветку активной (`git checkout имя`).
1. Необходимо разместить как исходные файлы с решениями задач, поместив **cpp** файлы в **src**, а заголовочные - в **include**. 
1. Добавить файлы в хранилище (`git add`).
1. Выполнить фиксацию изменений (`git commit -m "комментарий"`).
1. Отправить содержимое ветки в свой удаленный репозитарий (`git push origin имя_ветки`).
1. Создать пул-запрос в репозитарий группы и ждать результата от **GitHub Actions**.

