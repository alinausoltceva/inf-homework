# inf-homework
## Лабораторная работа: Команда grep
Лабораторная работа посвящена изучению возможностей команды grep для поиска и фильтрации данных в текстовых файлах с использованием регулярных выражений.

## Пример  
Создадим текстовый файл poem.txt с некоторым содержимым. Например:

Послушайте!  
Ведь, если звезды зажигают —  
значит — это кому-нибудь нужно?  
Значит — кто-то хочет, чтобы они были?  
Значит — кто-то называет эти плево́чки жемчужиной?

И, надрываясь  
в метелях полу́денной пыли,  
врывается к богу,  
боится, что опоздал,  
плачет,  
целует ему жилистую руку,  
просит —  
чтоб обязательно была звезда! —  
клянется —  
не перенесет эту беззвездную муку!  
А после  
ходит тревожный,  
но спокойный наружно.  
Говорит кому-то:  
«Ведь теперь тебе ничего?  
Не страшно?  
Да?!»  
Послушайте!  
Ведь, если звезды  
зажигают —  
значит — это кому-нибудь нужно?  
Значит — это необходимо,  
чтобы каждый вечер  
над крышами  
загоралась хоть одна звезда?!

Теперь попроубем найти строки этого файла, в которых содержится слова с корнем -звезд-. Для этого используем команду grep:

grep -o 'bw*звездw*b' poem.txt  
Должен получиться следующий вывод:

Ведь, если звезды зажигают —  
не перенесет эту беззвездную муку!  
Ведь, если звезды
загоралась хоть одна звезда?!

## Задание  
Вам дан файл oblako_v_shtanah.txt, в котором представлено содержание второй главы поэмы Маяковского "Облако в штанах":

Славьте меня!  
Я великим не чета.  
Я над всем, что сделано,  
ставлю «nihil».

Никогда  
ничего не хочу читать.  
Книги?  
Что книги!...
Найдите все строки, начинающиеся на слова "я", "мы" или "вы"  в любом регистре и до конца предложения.

## Источники  
https://google.com/
https://www.gnu.org/
