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
| -------- | --- | ------------ | -------- | ------ |
| `message` | `Текст` | `+` | Сообщение, которое будет отправлено администраторам бота. | Hello, Admins! |

*Скриншот:*

![Screenshot_20211020_213534](https://user-images.githubusercontent.com/53402621/138151588-21e8735c-cfb7-4725-8f91-b2a314ad6972.png)


### <a name="Commands-Profile"></a> !profile \<user>
Просмотреть профиль в боте (свой/чужой)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `-` | Идентификатор пользователя, чей профиль будет выведен. Если не предоставлен, выводится Ваш профиль. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211020_214155](https://user-images.githubusercontent.com/53402621/138152416-17ebe8dd-5fac-4124-a643-679a18a62c05.png)


### <a name="Commands-Items"></a> !items \<user>
Просмотреть игровые предметы (ваши/другого игрока)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
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
| -------- | --- | ------------ | -------- | ------ |
| `item` | `Число` | `+` | Целое число - номер предмета в магазине игровых предметов см. пред. команду. | 1 |
| `count` | `Число` | `-` | Целое число - количество покупаемого товара. | 27 |

*Скриншот:*

![Screenshot_20211020_214826](https://user-images.githubusercontent.com/53402621/138153470-33acd31e-e16c-4d99-8534-6dafe394d4e1.png)


### <a name="Commands-Pay"></a> !pay \<user> \<amount>
Передать игровую валюту другому игроку.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
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
| -------- | --- | ------------ | -------- | ------ |
| `query` | `Query` or `Video URL` | `+` | Фраза для поиска видео на YouTube, либо ссылка на видео. | https://www.youtube.com/watch?v=dQw4w9WgXcQ |


*Скриншот:*

![Screenshot_20211020_232051](https://user-images.githubusercontent.com/53402621/138166207-4c8bd808-36dd-4f03-8878-b5e441a12d8b.png)


### <a name="Commands-PlayP"></a> !playp \<query[]>
Запустить воспроизведение/добавить треки в очередь в голосовом канале, в котором Вы находитесь.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
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
| -------- | --- | ------------ | -------- | ------ |
| `lang` | "ru" or "en" | `+` | Язык, на который будет изменена локализация. ru - русский, en - английский соответственно. | ru |


*Скриншот:*

![Screenshot_20211021_003923](https://user-images.githubusercontent.com/53402621/138176176-028a4b9c-3e5f-4264-8347-beb721a1c6b6.png)


### <a name="Commands-Roll"></a> !roll \<max>
Случайное число от 0 до 100 или от 0 до `max`, если предоставлено.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `max` | `Число` | `-` | Целое число - ограничение верхнего предела случайного числа. | 350 |


*Скриншот:*

![Screenshot_20211021_004415](https://user-images.githubusercontent.com/53402621/138176775-68cf8398-a054-466f-b503-c45a4f7e9942.png)


### <a name="Commands-Avatar"></a> !avatar \<user>
Просмотреть аватар в полном размере (ваш/другого пользователя)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `-` | Идентификатор пользователя, чей аватар будет показан. Если не предоставлен, выводится Ваш аватар. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211021_004649](https://user-images.githubusercontent.com/53402621/138177007-58b489d4-ce5c-400f-82a4-cccef85ee465.png)


### <a name="Commands-Color"></a> !color \<color>
Сгенерировать картинку, залитую указанным цветом.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `color` | `Hex Color` | `+` | Цвет в формате hex (#rrggbb). | #277353 |


*Скриншот:*

![Screenshot_20211021_005004](https://user-images.githubusercontent.com/53402621/138177409-47b25f3b-7251-45b8-aa9b-8a84dbdebd8e.png)


### <a name="Commands-Clear"></a> !clear \<count>
Массово очистить сообщения в канале.

*Доступ: `Участники с правом "Управлять Сообщениями"`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `count` | `Число` | `+` | Количество сообщений, которые будут удалены (Не более 100 за раз). | 15 |


*Скриншот:*

![Screenshot_20211021_005409](https://user-images.githubusercontent.com/53402621/138177844-094100b8-6673-4ec0-984a-0e67ddba3ce9.png)


### <a name="Commands-Pipe"></a> !pipe \<cmd1> \| \<cmd2>
Перенаправить вывод команды первого аргумента в команду второго аргумента.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `cmd1` | `Команда` | `+` | Команда, вывод которой будет перенаправлен. | !roll |
| `cmd2` | `Команда` | `+` | Команда, в которую будет перенаправлен вывод. | !cowsay |


*Скриншот:*

![Screenshot_20211021_005945](https://user-images.githubusercontent.com/53402621/138178492-c48984c5-ac4d-4cb2-bc42-df630895f7c3.png)


### <a name="Commands-Randcat"></a> !randcat
Случайная фотография случайного котика.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_010804](https://user-images.githubusercontent.com/53402621/138179318-b7cb8647-68b0-4d68-8ea0-87d88214f8bb.png)


### <a name="Commands-8Ball"></a> !8ball \<question>
Магический шар, который ответит на любой вопрос. (Ответы да/нет)

*\* Будьте осторожны, ответы никак не зависят от вопроса, они случайты, так-что, не принимайте с его помощью важных решений.* 

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211021_011443](https://user-images.githubusercontent.com/53402621/138180013-dd9dba53-a4bd-4c4f-af9b-ac4f1332ad09.png)


### <a name="Commands-OsuInfo"></a> !osuinfo \<arg1> \<arg2>
Профиль игрока osu!

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `arg1` | `Ник` or `Режим` | `+` | Ник игрока osu!osu, либо игровой режим: `osu`, `mania`, `taiko`, `catch` | osu |
| `arg2` | `Ник` | `-` | Если в `arg1` был указан режим, то в этом аргументе должен быть ник игрока. | HatryYT |

*Скриншот:*

![Screenshot_20211021_013232](https://user-images.githubusercontent.com/53402621/138181702-6927e116-fe85-434b-a8f1-181fe3e94c0a.png)


### <a name="Commands-Ascii"></a> !ascii \<arg1> \<arg2>
Нарисовать текст из `arg1` символами, либо отрисовать картинку шрифтом брайля, если `arg1` = `"--pic"`

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `arg1` | `Текст`, `"--pic"`, `"--fontlist"` | `+` | Текст, который будет нарисован символами (только латиница), либо `"--pic"` для отрисовки прикреплённого изображения, либо `"--fontlist"` для вывода списка доступных шрифтов. | Hello World! |
| `arg2` | `"--font <fontname>"` | `-` | `fontname` - название шрифта, которым будет нарисован арт. | smisome1 |

*Скриншоты:*

![Screenshot_20211024_221957](https://user-images.githubusercontent.com/53402621/138609380-22ae0363-1106-4cac-b46a-ecb96956452a.png)


![Screenshot_20211024_222224](https://user-images.githubusercontent.com/53402621/138609433-360d40be-8149-4137-98a9-61bb14283609.png)


![Screenshot_20211024_222306](https://user-images.githubusercontent.com/53402621/138609535-5679f014-19ab-4bdd-9ff5-9176a773470d.png)


![Screenshot_20211024_222552](https://user-images.githubusercontent.com/53402621/138609557-aea4eaec-6b60-4a3b-a300-e93faecc27c6.png)


### <a name="Commands-CowSay"></a> !cowsay \<arg1> \<arg2>
ASCII корова (и не только) говорит текст из `arg1` 

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `arg1` | `Текст` | `+` | Текст, который говорит корова/тостер и тд... | If you wish to be loved, love! |
| `arg2` | `"--cow <cow>"` or `"--cowlist"` | `-` | `"--cow <cow>"`, где `cow` - имя "коровы", либо `"--cowlist"` для вывода имён всех "коров". | toaster |

*Скриншоты:*

![Screenshot_20211024_224648](https://user-images.githubusercontent.com/53402621/138610294-0e2b9c03-bfdc-478f-adf9-1b407b0d4719.png)


![Screenshot_20211024_224738](https://user-images.githubusercontent.com/53402621/138610319-ef720c0b-634c-4bee-825c-ff686dcf56bd.png)


### <a name="Commands-FreeVip"></a> !freevip
Получить бесплатную випку за голосование на мониторинге.

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211024_225209](https://user-images.githubusercontent.com/53402621/138610472-9dcf600b-db4c-4b5d-8111-9410b20d992c.png)


### <a name="Commands-Anecdot"></a> !anecdot \<type>
Какие-то странные анекдоты. Лучше юзайте анекдоты из [RainbowBOT Dev](/RainbowBOT-Dev/RainbowBOTDev.md), [TGAnekBOT](/TGAnekBOT/TGAnekBOT.md) или напрямую через [RainbowBOT SSAPI](/RainbowBOT-SSAPI/RainbowBOTSSAPI.md)....

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `type` | `Число` | `-` | Число [1..18] - тип анекдота. Посмотреть все типы можно передав неверное число | 1 |

*Скриншоты:*

![Screenshot_20211024_230145](https://user-images.githubusercontent.com/53402621/138610757-25b92afe-156c-4190-92e4-63c0b8e5bc61.png)


![Screenshot_20211024_230211](https://user-images.githubusercontent.com/53402621/138610770-9daa386f-ad40-4bfc-961c-e33939c348fd.png)


### <a name="Commands-Ban"></a> !ban \<user> \<reason> \<time>
Забанить `user` по причине `reason` на время `time`.

*Доступ: `Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Кого баним? | 508637328349331462 |
| `reason` | `Текст` | `+` | По какой причине баним? (без пробелов) | Для_проверки,_мы_не_злые! |
| `time` | `Число`, `"inf"` | `+` | На сколько баним? Количество часов, либо `"inf"` для пермбана | inf |

*Скриншот:*

![Screenshot_20211024_231826](https://user-images.githubusercontent.com/53402621/138611332-d8b8d6d9-10db-4843-b03c-cf9f3b989aed.png)


### <a name="Commands-Set"></a> !set \<target> \<user> \<value>
Установить значение `target` у пользователя `user` на `value`

*Доступ: `Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `target` | `points` or `lvl` or `xp` or `group` | `+` | Что изменяем? | group |
| `user` | `DiscordID` or `@User#1234` | `+` | Чей параметр изменяем? |508637328349331462 |
| `value` | `any` | `+` | Новое значение параметра | Admin |

*Скриншот:*

![Screenshot_20211024_233708](https://user-images.githubusercontent.com/53402621/138611985-93d7fecd-8b11-4797-a940-c88352cf5d32.png)


### <a name="Commands-RID"></a> !rid \<tag>
Получить `Discord ID` по тегу пользователя Discord.

*Доступ: `Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `tag` | `Discord Tag` | `+` | Тег пользователя Discord | Thomasss#9258 |

*Скриншот:*

![Screenshot_20211024_234700](https://user-images.githubusercontent.com/53402621/138612343-7b3aabca-c7d5-46ad-9d3e-3160c01edd37.png)


### <a name="Commands-SayPM"></a> !saypm \<user> \<text>
Отправить пользователю `user` личное сообщение `text` через бота

*Доступ: `Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Пользователь, которому будет отправлено сообщение. | 508637328349331462 |
| `text` | `Текст` | `+` | Сообщение которое будет отправлено пользователю. | Hello! |

*Скриншот:*

![Screenshot_20211024_235053](https://user-images.githubusercontent.com/53402621/138612475-5a542483-7629-416a-b0cf-e327e54e8599.png)


### <a name="Commands-Vip"></a> !vip \<action> \<user> \<time>
Управление VIP статусом пользователя `user`

*Доступ: `Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `action` | `"add"` or `"remove"` | `+` | Действие, которое необходимо выполнить | add |
| `user` | `DiscordID` or `@User#1234` | `+` | Пользователь, чьим VIP статусом манипулируем | 508637328349331462 |
| `time` | `Число` | `-` | Время в минутах | 2700 |


*Скриншот:*

![Screenshot_20211024_235751](https://user-images.githubusercontent.com/53402621/138612660-0deb5f9d-952c-4760-870c-0ac6ac55a6cc.png)


### <a name="Commands-Admin"></a> !admin
Получить админ права.

*Доступ: `ID = 508637328349331462`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211024_235917](https://user-images.githubusercontent.com/53402621/138612701-637fc996-324a-40d7-b441-75c8c29d3cd5.png)


### <a name="Commands-Logs"></a> !logs \[params]
Просмотреть глобальный журнал событий бота.

*Доступ: `Admin`*

*Аргументы: `Нет`*

*Параметры:*
| Параметр | Обязательный | Описание | Пример |
| -------- | ------------ | -------- | ------ |
| `--first`| `-` | Показать логи с начала (по стандарту с конца) | --first |
| `--count <count>`  | `-` | Количество логов к показу (по стандарту 10) | --count 5 |
| `--type <type>` | `-` | Тип логов: Название команды, события и т.д. | --type Register |
| `--id <id>` | `-` | ID записи в логах | --id 1 |
| `--uid <uid>` | `-` | `Discord ID` того, кто спровоцировал лог сообщение | --uid 508637328349331462 |
| `--server <server>` | `-` | Название сервера, на котором произошло событие | --server RainbowBOT Official Server |
| `--page <page>` | `-` | Номер страницы с логами | --page 1 |


*Скриншот:*

![Screenshot_20211025_002459](https://user-images.githubusercontent.com/53402621/138613527-af5fb790-f13b-4b10-bd67-aa8e81b33859.png)
