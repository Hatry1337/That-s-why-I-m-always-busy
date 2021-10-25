# RainbowBOT - Discord-бот с широким функционалом.

Оглавление |
| - |
| [О боте](#About) |
| [Команды](#Commands) |
|   Info |
| [    !rhelp](#Commands-RHelp) |
| [    !usage](#Commands-Usage) |
|   Utility |
| [    !joinmgr](#Commands-JoinMGR) |
| [    !leavemgr](#Commands-LeaveMGR) |
| [    !rbfetch](#Commands-RBFetch) |
| [    !config](#Commands-Config) |
| [    !vl](#Commands-VL) |
| [    !music](#Commands-Music) |
| [    !avatar](#Commands-Avatar) |
|   Moderation |
| [    !mute](#Commands-Mute) |
| [    !unmute](#Commands-UnMute) |
| [    !clear](#Commands-Clear) |
|   Fun |
| [    !anek](#Commands-Anek) |

## <a name="About"></a> О боте 
RainbowBOT Dev - ответвление основного бота, которое позже было полностью переписано на TypeScript, была переработана вся архитектура и был применён полностью модульный подход к разработке. Позже этот бот заменит собой классического RainbowBOT JS.

Как было сказано выше - бот написан на TypeScript с использованием Discord.js 13, Node.js, PostgreSQL, Sequelize. Изначально задумывался как унифицированняя платформа для ботов, но пока не сложилось. 

## <a name="Commands"></a> Команды 

### <a name="Commands-RHelp"></a> !rhelp \<page> \<category>
Команда помощи по использованию бота, выводит список команд, их описание, использование.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `page` | `Число` | `-` | Номер страницы списка команд | 2 |
| `category` | `Category` | `-` | Позволяет выводить только команды определенной категории | Moderation |


*Скриншоты:*

![Screenshot_20211025_213753](https://user-images.githubusercontent.com/53402621/138751391-930af5f3-49ad-4e76-a4f0-e535d1d357e4.png)


![Screenshot_20211025_213857](https://user-images.githubusercontent.com/53402621/138751482-22c3217a-0711-4c9e-80ed-fed51ffbc06d.png)


### <a name="Commands-Uptime"></a> !usage <command>
Позволяет просмотреть подробное описание команды, с примерами использования.

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `command` | `Command` | `+` | Название команды, информацию о которой нужно узнать | !joinmgr |

*Скриншот:*

![Screenshot_20211025_215204](https://user-images.githubusercontent.com/53402621/138753142-d1dbc523-eba7-4f11-940b-9fe6b4670df8.png)



### <a name="Commands-JoinMGR"></a> !joinmgr \<subc> ...
Позволяет настроить автовыдачу ролей, вывод приветственного сообщения при подключении к серверу.

*Доступ: `Server Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `subc` | `SubCmd` | `+` | Подкоманда, которую требуется выполнить | join-roles |

*SubCmds:*
| Подкоманда | Описание | Пример |
| ---------- | -------- | ------ |
| add-join-role `@role` | Добавляет указанную роль в список ролей для автовыдачи. Максимум ролей для автовыдачи: 20 | !joinmgr add-join-role @Player |
| rm-join-role `@role` | Удаляет указанную роль из списка ролей для автовыдачи. | !joinmgr rm-join-role @Player |
| join-roles | Выводит список ролей для автовыдачи. | !joinmgr join-roles |
| join-message-channel `#channel` | Устанавливает указанный канал для приветственных сообщений | !joinmgr join-message-channel #join-messages |
| join-message-cfg | Запускает мастер настройки приветственного сообщения | !joinmgr join-message-cfg |
| join-message-enable | Включает приветственное сообщение на сервере. | !joinmgr join-message-enable |
| join-message-disable | Выключает приветственное сообщение на сервере. | !joinmgr join-message-disable |



*Скриншоты:*

![Screenshot_20211025_220954](https://user-images.githubusercontent.com/53402621/138755385-e52666f2-57bc-490e-9e00-63180f07fed1.png)


![Screenshot_20211025_221020](https://user-images.githubusercontent.com/53402621/138755442-403ce115-ef98-4bb6-a140-5210aa9cdccf.png)


![Screenshot_20211025_221124](https://user-images.githubusercontent.com/53402621/138755565-964246fb-990d-402b-a0ed-efc25593bab2.png)


## <a name="Commands-LeaveMGR"></a> !leavemgr \<subc> ...
Позволяет настроить автоматическое сообщение при выходе с сервера.

*Доступ: `Server Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `subc` | `SubCmd` | `+` | Подкоманда, которую требуется выполнить | leave-message-channel |

*SubCmds:*
| Подкоманда | Описание | Пример |
| ---------- | -------- | ------ |
| leave-message-channel `#channel` | Устанавливает указанный канал для сообщений о выходе с сервера. | !leavemgr leave-message-channel #leave-messages |
| leave-message-cfg | Запускает мастер настройки сообщения о выходе с сервера. | !leavemgr leave-message-cfg |
| leave-message-enable | Включает сообщение о выходе с сервера. | !leavemgr leave-message-enable |
| leave-message-disable | Выключает сообщение о выходе с сервера. | !leavemgr leave-message-disable |


*Скриншот:*

![Screenshot_20211025_222101](https://user-images.githubusercontent.com/53402621/138756877-e36b0b45-1892-4fcc-a0ef-3fb9c06f7628.png)


### <a name="Commands-RBFetch"></a> !rbfetch
Информация о различных параметрах бота стилизованная под линуксовый neofetch/screenfetch

*Доступ: `Все`*

*Аргументы: `Нет`*

*Скриншот:*

![Screenshot_20211025_222857](https://user-images.githubusercontent.com/53402621/138757992-128f6491-cd4a-49bc-b61d-d09d6702184b.png)


## <a name="Commands-Config"></a> !config \<subc> ...
Позволяет настроить константные параметры бота.

*Доступ: `Server Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `subc` | `SubCmd` | `+` | Подкоманда, которую требуется выполнить | muted-role |

*SubCmds:*
| Подкоманда | Описание | Пример |
| ---------- | -------- | ------ |
| muted-role `@role` | Устанавливает роль, которая будет выдаваться при муте пользователей. Если роль не передана, создастся новая. | !config muted-role |
| mod-role `@role` | Устанавливает модераторскую роль | !config mod-role @Moder |


*Скриншот:*

![Screenshot_20211025_223718](https://user-images.githubusercontent.com/53402621/138759099-9cc59a11-24b4-4c96-b779-cd7aa4a6b546.png)


## <a name="Commands-VL"></a> !vl \<subc> ...
Позволяет настраивать персональные голосовые комнаты на сервере.

*Доступ: `Server Admin`, `Lobby Creator`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `subc` | `SubCmd` | `+` | Подкоманда, которую требуется выполнить | muted-role |

*SubCmds:*
| Подкоманда | Доступ | Описание | Пример |
| ---------- | ------ | -------- | ------ |
| setup | `Server Admin` | Сконфигурировать голосовые комнаты на сервере | !vl setup |
| destroy | `Server Admin` | Очистить имеющуюся конфигурацию голосовых комнат | !vl destroy |
| invite `@user` | `Lobby Creator` | Пригласить пользователя в Вашу приватную комнату | !vl invite @Thomasss |
| kick `@user` | `Lobby Creator` | Выгнать пользователя из Вашей приватной комнаты | !vl kick @Thomasss |
| public | `Lobby Creator` | Сделать Вашу комнату публичной | !vl public |
| private | `Lobby Creator` | Сделать Вашу комнату приватной | !vl private |


*Скриншоты:*

![Screenshot_20211025_230159](https://user-images.githubusercontent.com/53402621/138762420-77ea2cee-df7f-4c24-a48e-425fc72f878e.png)


![Screenshot_20211025_230235](https://user-images.githubusercontent.com/53402621/138762485-6b7f082e-e86e-4ddb-bf87-58fc9226f355.png)


![Screenshot_20211025_230253](https://user-images.githubusercontent.com/53402621/138762539-6991f13a-78f6-4cce-acd4-67b50af92ce8.png)


## <a name="Commands-Music"></a> !music \<subc> ...
Позволяет сконфигурировать музыкальный плеер на сервере.

*Доступ: `Server Admin`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `subc` | `SubCmd` | `+` | Подкоманда, которую требуется выполнить | muted-role |

*SubCmds:*
| Подкоманда | Описание | Пример |
| ---------- | -------- | ------ |
| setup | Сконфигурировать музыкальный плеер на этом сервере. | !music setup |

*Скриншоты:*

![Screenshot_20211025_231711](https://user-images.githubusercontent.com/53402621/138764461-964ed3a1-e7a1-4a82-a272-aa288755654a.png)


![Screenshot_20211025_231859](https://user-images.githubusercontent.com/53402621/138764702-8755f7d0-6766-4e1d-991d-1efacadf1cee.png)


### <a name="Commands-Avatar"></a> !avatar \<user>
Просмотреть аватар в полном размере (ваш/другого пользователя)

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Идентификатор пользователя, чей аватар будет показан. Если не предоставлен, выводится Ваш аватар. | 508637328349331462 |

*Скриншот:*

![Screenshot_20211025_232428](https://user-images.githubusercontent.com/53402621/138765478-437f7460-f8ea-44bc-af46-1c76ac4d204e.png)


### <a name="Commands-Mute"></a> !mute \<user> \<time> \<reason>
Замутить пользователя `user` на `time` по причине `reason`

*Доступ: `Moderator`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Идентификатор пользователя, которого нужно замутить | 508637328349331462 |
| `time` | `CombTime` | `+` | Время, на которое нужно замутить `1d`, `1h`, `1m`, `1s`, `perm` (можно комбинировать) | 1d12h |
| `reason` | `Текст` | `+` | Причина мута | Тестируем типа.. |


*Скриншот:*

![Screenshot_20211025_233735](https://user-images.githubusercontent.com/53402621/138767219-6767f29f-1465-4289-9ad1-182564bf9dbb.png)


### <a name="Commands-UnMute"></a> !unmute \<user>
Размутить пользователя `user`

*Доступ: `Moderator`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `user` | `DiscordID` or `@User#1234` | `+` | Идентификатор пользователя, которого нужно размутить | 508637328349331462 |

*Скриншот:*

![Screenshot_20211025_233806](https://user-images.githubusercontent.com/53402621/138767281-4abeaffb-cfc7-4967-9b9c-bccc00d9bc5b.png)


### <a name="Commands-Clear"></a> !clear \<count>
Массово очистить сообщения в канале.

*Доступ: `Участники с правом "Управлять Сообщениями"`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `count` | `Число` | `+` | Количество сообщений, которые будут удалены (Не более 100 за раз). | 15 |


*Скриншот:*

![Screenshot_20211021_005409](https://user-images.githubusercontent.com/53402621/138177844-094100b8-6673-4ec0-984a-0e67ddba3ce9.png)


### <a name="Commands-Anek"></a> !anek \<arg1> \<arg2>
Анекдоты. Категории Б. Что может быть лучше?

*Доступ: `Все`*

*Аргументы:*
| Аргумент | Тип | Обязательный | Описание | Пример |
| -------- | --- | ------------ | -------- | ------ |
| `arg1` | `Tag` or `"id"` or `"tags"` | `-` | Случайный анек по тегу из `arg1`, либо по id из `arg2`, если `arg1` = `"id"`, либо список всех тегов если `arg1` = `"tags"` |  |


*Скриншот:*

![Screenshot_20211025_234751](https://user-images.githubusercontent.com/53402621/138768551-db018573-af7c-45be-b199-3177f6e2bd69.png)


![Screenshot_20211025_234832](https://user-images.githubusercontent.com/53402621/138768652-612dfcd5-34c3-4ab7-952f-b776a0c1bb85.png)