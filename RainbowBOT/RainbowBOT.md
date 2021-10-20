# RainbowBOT - Discord-бот с широким функционалом.

Оглавление |
| - |
| [О боте](#About) |
| [Команды](#Commands) |
|   Информационные |
| [    !rhelp](#Commands-RHelp) |
| [    !uptime](#Commands-Uptime) |
| [    !rstats](#Commands-RStats) |
| [    !rep](#Commands-Rep) |
|   Экономика |
| [    !profile](#Commands-Profile) |
| [    !items](#Commands-Items) |
| [    !shop](#Commands-Shop) |
| [    !buy](#Commands-Buy) |
| [    !pay](#Commands-Pay) |
| [    !getmoney](#Commands-Getmoney) |
| [    !top](#Commands-Top) |
|   Музыка \[DEPRECATED] |
| [    !play](#Commands-Play) |
| [    !playp](#Commands-PlayP) |
| [    !stop](#Commands-Stop) |
| [    !skip](#Commands-Skip) |
| [    !repeat](#Commands-Repeat) |
| [    !rbfm](#Commands-RBFM) |
| [    !queue](#Commands-Queue) |
|   Утилиты |
| [    !lang](#Commands-Lang) |
| [    !roll](#Commands-Roll) |
| [    !avatar](#Commands-Avatar) |
| [    !color](#Commands-Color) |
| [    !clear](#Commands-Clear) |
| [    !pipe](#Commands-Pipe) |
|   Прочие |
| [    !randcat](#Commands-Randcat) |
| [    !8ball](#Commands-8Ball) |
| [    !osuinfo](#Commands-OsuInfo) |
| [    !ascii](#Commands-Ascii) |
| [    !cowsay](#Commands-CowSay) |
| [    !freevip](#Commands-FreeVip) |
| [    !anecdot](#Commands-Anecdot) |
|   Админские |
| [    !ban](#Commands-Ban) |
| [    !set](#Commands-Set) |
| [    !rid](#Commands-RID) |
| [    !saypm](#Commands-SayPM) |
| [    !vip](#Commands-Vip) |
| [    !admin](#Commands-Admin) |
| [    !logs](#Commands-Logs) |



## <a name="About"></a> О боте 
В данный момент разработка в главной ветке не ведётся, выходят лишь критические исправления. Основные силы брошены на портирование функционала на новую базу ([RainbowBOT DEV](https://github.com/Hatry1337/That-s-why-I-m-always-busy/RainbowBOT-DEV.md)).
RainbowBOT написан на JavaScript и использует Node.js, Discord.js, MySQL. Пригласить бота на свой сервер можно по ссылке https://rainbowbot.xyz/invite

## <a name="Commands"></a> Команды 

### <a name="Commands-RHelp"></a> !rhelp
Команда помощи по использованию бота, выводит список команд, их описание, использование.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![rbot-rhelp](https://user-images.githubusercontent.com/53402621/138149398-0a4c4402-4ec2-444d-a5fb-bd9291a2d7f1.png)

### <a name="Commands-Uptime"></a> !uptime
Выводит информацию о времени работы бота с момента включения.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211020_212406](https://user-images.githubusercontent.com/53402621/138149782-39d23334-d9e7-4311-a616-307b05bb5555.png)


### <a name="Commands-RStats"></a> !rstats
Выводит статистическую информацию о различных параметрах бота.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211020_212544](https://user-images.githubusercontent.com/53402621/138150021-168637ec-9e33-417e-ae33-7580e6840203.png)


### <a name="Commands-Rep"></a> !rep \<message>
Отправить сообщение администраторам бота

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `message` | `Текст` | `+` | Сообщение, которое будет отправлено администраторам бота. | Hello, Admins! |

*Скриншот:*

![Screenshot_20211020_213534](https://user-images.githubusercontent.com/53402621/138151588-21e8735c-cfb7-4725-8f91-b2a314ad6972.png)


### <a name="Commands-Profile"></a> !profile \<user>
Просмотреть профиль в боте (свой/чужой)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `user` | `DiscordID` or `@User#1234` | `-` | Идентификатор пользователя, чей профиль будет выведен. Если не предоставлен, выводится Ваш профиль. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211020_214155](https://user-images.githubusercontent.com/53402621/138152416-17ebe8dd-5fac-4124-a643-679a18a62c05.png)


### <a name="Commands-Items"></a> !items \<user>
Просмотреть игровые предметы (ваши/другого игрока)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `user` | `DiscordID` or `@User#1234` | `-` | Идентификатор пользователя, чьи игровые предметы будут показаны. Если не предоставлен, выводятся Ваши предметы. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211020_215514](https://user-images.githubusercontent.com/53402621/138154351-4f5b05d0-8c44-4965-bc78-cff48bb505e6.png)


### <a name="Commands-Shop"></a> !shop
Список товаров в магазине игровых предметов.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211020_214528](https://user-images.githubusercontent.com/53402621/138152923-9541d327-39b3-4926-9550-8cb763e13324.png)


### <a name="Commands-Buy"></a> !buy \<item> \<count>
Купить предмет из магазина игровых предметов.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `item` | `Число` | `+` | Целое число - номер предмета в магазине игровых предметов см. пред. команду. | 1 |
| `count` | `Число` | `-` | Целое число - количество покупаемого товара. | 27 |

*Скриншот:*

![Screenshot_20211020_214826](https://user-images.githubusercontent.com/53402621/138153470-33acd31e-e16c-4d99-8534-6dafe394d4e1.png)


### <a name="Commands-Pay"></a> !pay \<user> \<amount>
Передать игровую валюту другому игроку.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Идентификатор пользователя, кому будет отправлена валюта. | 508637328349331462 |
| `amount` | `Число` | `+` | Целое число - количество передаваемой валюты. | 1000 |


*Скриншот:*

![Screenshot_20211020_220128](https://user-images.githubusercontent.com/53402621/138155287-9a248364-d33e-4a54-9df9-ff8b923c7b34.png)


### <a name="Commands-Getmoney"></a> !getmoney
Снять поинты с Bitcoin-майнеров.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211020_221148](https://user-images.githubusercontent.com/53402621/138156745-a33b89b7-f214-4416-b467-a31609a93ed7.png)


### <a name="Commands-Top"></a> !top
Таблица лидеров по игровой валюте.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211020_230130](https://user-images.githubusercontent.com/53402621/138163475-97c41477-f299-42d8-8cda-a150d7fff6f3.png)


### <a name="Commands-Play"></a> !play \<query>
Запустить воспроизведение/добавить трек в очередь в голосовом канале, в котором Вы находитесь.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `query` | `Query` or `Video URL` | `+` | Фраза для поиска видео на YouTube, либо ссылка на видео. | https://www.youtube.com/watch?v=dQw4w9WgXcQ |


*Скриншот:*

![Screenshot_20211020_232051](https://user-images.githubusercontent.com/53402621/138166207-4c8bd808-36dd-4f03-8878-b5e441a12d8b.png)


### <a name="Commands-PlayP"></a> !playp \<query[]>
Запустить воспроизведение/добавить треки в очередь в голосовом канале, в котором Вы находитесь.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `query` | `Query[]` or `Video URL[]` | `+` | Ссылки/поисковые запросы на видео объединенные в одну команду, разделённые с помощью `;;`. | https://www.youtube.com/watch?v=dQw4w9WgXcQ;;https://www.youtube.com/watch?v=xkIICPm9nag |


*Скриншот:*

![Screenshot_20211020_232051](https://user-images.githubusercontent.com/53402621/138166207-4c8bd808-36dd-4f03-8878-b5e441a12d8b.png)


### <a name="Commands-Stop"></a> !stop
Остановить воспроизведение, очистить очередь воспроизведения.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_000021](https://user-images.githubusercontent.com/53402621/138171317-901c01ec-079f-489f-8ab0-87eae71d2a92.png)


### <a name="Commands-Skip"></a> !skip
Пропустить текущий трек, начать играть следующий из очереди.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_000200](https://user-images.githubusercontent.com/53402621/138171539-b14b150f-160e-4996-8ef6-bd80b0ea3aba.png)


### <a name="Commands-Repeat"></a> !repeat
Зациклить воспроизведение текущего трека.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_000343](https://user-images.githubusercontent.com/53402621/138171790-f907d667-3946-4faa-8ade-add4f2e60014.png)


### <a name="Commands-RBFM"></a> !rbfm
Воспроизвести интернет-радио поток [RainbowFM](/RainbowFM.md) 

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_000706](https://user-images.githubusercontent.com/53402621/138172271-edd828ac-184e-43a2-b538-3ad721f48336.png)


### <a name="Commands-Queue"></a> !queue
Показать очередь воспроизведения

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_000434](https://user-images.githubusercontent.com/53402621/138171905-0b66f9ad-2434-4d06-a234-95eba61cfd45.png)


### <a name="Commands-Lang"></a> !lang \<lang>
Сменить язык бота.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `lang` | "ru" or "en" | `+` | Язык, на который будет изменена локализация. ru - русский, en - английский соответственно. | ru |


*Скриншот:*

![Screenshot_20211021_003923](https://user-images.githubusercontent.com/53402621/138176176-028a4b9c-3e5f-4264-8347-beb721a1c6b6.png)


### <a name="Commands-Roll"></a> !roll \<max>
Случайное число от 0 до 100 или от 0 до `max`, если предоставлено.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `max` | `Число` | `-` | Целое число - ограничение верхнего предела случайного числа. | 350 |


*Скриншот:*

![Screenshot_20211021_004415](https://user-images.githubusercontent.com/53402621/138176775-68cf8398-a054-466f-b503-c45a4f7e9942.png)


### <a name="Commands-Avatar"></a> !avatar \<user>
Просмотреть аватар в полном размере (ваш/другого пользователя)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `user` | `DiscordID` or `@User#1234` | `-` | Идентификатор пользователя, чей аватар будет показан. Если не предоставлен, выводится Ваш аватар. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211021_004649](https://user-images.githubusercontent.com/53402621/138177007-58b489d4-ce5c-400f-82a4-cccef85ee465.png)


### <a name="Commands-Color"></a> !color \<color>
Сгенерировать картинку, залитую указанным цветом.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `color` | `Hex Color` | `+` | Цвет в формате hex (#rrggbb). | #277353 |


*Скриншот:*

![Screenshot_20211021_005004](https://user-images.githubusercontent.com/53402621/138177409-47b25f3b-7251-45b8-aa9b-8a84dbdebd8e.png)


### <a name="Commands-Clear"></a> !clear \<count>
Массово очистить сообщения в канале.

*Доступ: `Участники с правом "Управлять Сообщениями"`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `count` | `Число` | `+` | Количество сообщений, которые будут удалены (Не более 100 за раз). | 15 |


*Скриншот:*

![Screenshot_20211021_005409](https://user-images.githubusercontent.com/53402621/138177844-094100b8-6673-4ec0-984a-0e67ddba3ce9.png)


### <a name="Commands-Pipe"></a> !pipe \<cmd1> \| \<cmd2>
Перенаправить вывод команды первого аргумента в команду второго аргумента.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| ------ | ------ | ------ | ------ | ------ |
| `cmd1` | `Команда` | `+` | Команда, вывод которой будет перенаправлен. | !roll |
| `cmd2` | `Команда` | `+` | Команда, в которую будет перенаправлен вывод. | !cowsay |


*Скриншот:*

![Screenshot_20211021_005945](https://user-images.githubusercontent.com/53402621/138178492-c48984c5-ac4d-4cb2-bc42-df630895f7c3.png)

