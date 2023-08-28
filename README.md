## Задание для PHP backend заработчика

Написать небольшую систему тикетов, используя nginx, PHP 8 и Laravel 9+. Система должна позволять добавлять новый тикет, а также оставлять комментарии в текущих.

Обязательные требования:
1. Данные нужно хранить в базе SQLite
2. Должна быть возможность зарегистрироваться, указав email и имя
3. После регистрации должно быть можно:
  - Просматривать историю своих тикетов
  - Создавать новый тикет
  - Комментировать и закрывать свои открытые тикеты
4. Должен быть создан аккаунт администратора, который имеет доступ ко всем тикетам
5. Тикет обязательно должен содержать
  - тип (выбор из списка)
  - текст (html-теги запрещены)
  - статус (new, in progress, closed)
6. Валидация вводимых данных на стороне клиента и сервера

Дополнительные требования:
1. К тикету можно приложить до 3 файлов общим размером не больше 5 MB; файлы должно быть можно посмотреть и/или скачать
2. Использовать для создания базы и добавления стандартного аккаунта администратора Laravel migration
3. Использовать ajax для добавления/обновления комментариев в тикете
4. Возможность администратору менять типы тикетов добавляя, редактируя или удаляя их
5. Возможность сортировать, фильтровать и искать по любому полю в списке тикетов
6. Возможность оставить комментарий или закрыть тикет сразу из таблицы тикетов (только если тикет ещё не закрыт)
7. Все формы отправки данных защитить от CSRF

## Uzdevums PHP backend izstrādātājam

Uztaisīt nelielu tiketu sistēmu, izmantojot nginx, PHP 8 un Laravel 9+. Sistēmai jāļauj pievienot jaunu tiketu, kā arī komentēt citos.

Obligātās prasības:
1. Dati jāglabā SQLite datubāzē
2. Jābūt iespējai reģistrēties, norādot vārdu un epastu
3. Pēc reģistrācijas jābūt atļautam:
  - Skatīt savu tiketu vēsturi
  - Izveidot jaunu tiketu
  - Komentēt un slēgt savus atvērtus tiketus
4. Jābūt izveidots administratora konts, kuram ir pieeja visiem tiketiem
5. Tiketam obligāti jābūt:
  - tips (izvēle no saraksta)
  - teksts (HTML-tagi ir aizliegti)
  - status (new, in progress, closed)
6. Datu validēšana klienta un servera pusē

Papildus prasības:
1. Tiketam var pievienot līdz 3 failiem ar kopējo izmēru ne vairāk 5 MB; jābūt iespējai failus apskatīt un/vai lejupielādēt
2. Datubāzes un administratora konta izveidei izmantot Laravel migration
3. Izmantot ajax komentāru pievienošanai/atjaunošanai tiketā
4. Iespēja administratoram mainīt tiketa tipus pievienojot, rediģējot vai dzēšos tos
5. Iespēja šķirot, filtrēt un meklēt izmantojot visus laukus tiketu sarakstā
6. Iespēja pievienot komentāru un slēgt tiketu no tiketu saraksta (ja tas vēl nav slēgts)
7. Visam datu sūtīšanas formām jābūt aizsargātam no CSRF
