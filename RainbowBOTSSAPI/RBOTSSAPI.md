# RainbowBOT Server Side API - Интерфейс взаимодействия с ботом и не только

Оглавление |
| - |
| [Что это?](#About) |
| [RainbowBOT API](#RBOTAPI) |
| [  /stats](#RBOTAPI-stats) |
| [  /userinfo](#RBOTAPI-userinfo) |
| [  /tops/servers/byactivity](#RBOTAPI-tops-servers-byactivity) |
| [  /tops/users/byactivity](#RBOTAPI-tops-users-byactivity) |
| [  /tops/users/bylvl](#RBOTAPI-tops-users-bylvl) |
| [  /tops/users/bypoints](#RBOTAPI-tops-users-bypoints) |
| [BAneks API](#BAneks) |
| [  /random](#BAneks-random) |
| [  /tag](#BAneks-tag) |
| [  /id](#BAneks-id) |
| [  /tags](#BAneks-tags) |


## <a name="About"></a> Что это?
RainbowBOT Server Side API - Открытый интерфейс для прямого взаимодействия с ботом и некоторыми утилитами. 

Все данные сериализуются в **JSON**.

## <a name="RBOTAPI"></a> RainbowBOT API
Статистика, информация RainbowBOT'а.

**BaseURL** - `api.rainbowbot.xyz/bot`

### <a name="RBOTAPI-stats"></a> [GET] /stats
Общая статистическая информация о боте.

*Структура ответа:*
```json
{
   "userscount"   : number,
   "msgcount"     : number,
   "msgcountday"  : number,
   "hentaicount"  : number,
   "regcountday"  : number,
   "totalpoints"  : number,
   "serverscount" : number,
   "botping"      : number
}
```

| Поле | Описание |
| ---- | -------- |
| `userscount` | Количество зарегистрированных пользователей в базе данных. |
| `msgcount` | Количество обработанных ботом сообщений (команд). (Всё время) |
| `msgcountday` | Количество обработанных ботом сообщений (команд). (Текущий день) |
| `hentaicount` | Количество хентайных картинок в базе данных. |
| `regcountday` | Количество зарегистрированных пользователей за текущий день. |
| `totalpoints` | Количество поинтов в обороте (на счетах всех пользователей). |
| `serverscount` | Количество Discord серверов, на которых находится бот. |
| `botping` | Задержка сокета взаимодействия бота с Discord API. |


### <a name="RBOTAPI-userinfo"></a> [GET] /userinfo/:DiscordID
Информация о пользователе по `DiscordID`.

*Структура ответа:*
```json
{
    "Username" : string,
    "Group"    : string,
    "Points"   : number,
    "Lvl"      : number,
    "XP"       : number,
    "ID"       : number,
    "Lang"     : string
}
```
| Поле | Описание |
| ---- | -------- |
| `Username` | Discord тэг пользователя. |
| `Group` | Группа пользователя (Admin, Player, VIP, etc.) |
| `Points` | Количество поинтов на счету у пользователя |
| `Lvl` | Уровень пользователя. |
| `XP` | Количество опыта у пользователя. |
| `ID` | Внутренний ID в боте. |
| `Lang` | Язык пользователя (ru, en). |


### <a name="RBOTAPI-tops-servers-byactivity"></a> [GET] /tops/servers/byactivity
Топ 100 серверов по количеству сообщений (команд).

*Структура ответа:*
```json
[
    {
        "server"   : string,
        "messages" : number
    }
]
```
| Поле | Описание |
| ---- | -------- |
| `server` | Название сервера. |
| `messages` | Количество сообщений на сервере. |


### <a name="RBOTAPI-tops-users-byactivity"></a> [GET] /tops/servers/byactivity
Топ 100 пользователей по количеству сообщений (команд).

*Структура ответа:*
```json
[
    {
        "username" : string,
        "messages" : number
    }
]
```
| Поле | Описание |
| ---- | -------- |
| `username` | Discord тэг пользователя. |
| `messages` | Количество сообщений на сервере. |


### <a name="RBOTAPI-tops-users-bylvl"></a> [GET] /tops/users/bylvl
Топ 100 пользователей по уровню.

*Структура ответа:*
```json
[
    {
        "username" : string,
        "points"   : number,
        "lvl"      : number
    }
]
```
| Поле | Описание |
| ---- | -------- |
| `username` | Discord тэг пользователя. |
| `points` | Количество поинтов пользователя. |
| `lvl` | Уровень пользователя. |


### <a name="RBOTAPI-tops-users-bypoints"></a> [GET] /tops/users/bypoints
Топ 100 пользователей по поинтам.

*Структура ответа:*
```json
[
    {
        "username" : string,
        "points"   : number,
        "lvl"      : number
    }
]
```
| Поле | Описание |
| ---- | -------- |
| `username` | Discord тэг пользователя. |
| `points` | Количество поинтов пользователя. |
| `lvl` | Уровень пользователя. |


## <a name="BAneks"></a> BAneks API
База анекдотов категории Б. Есть теги!!

**BaseURL** - `api.rainbowbot.xyz/baneks`

### <a name="BAneks-random"></a> [GET] /random
Случайный анекдот категории Б.

*Структура ответа:*
```json
{
   "status" : number,
   "id"     : number,
   "anek"   : string,
   "source" : string,
   "s_id"   : string,
   "views"  : number,
   "tags"   : string[]
}
```

| Поле | Описание |
| ---- | -------- |
| `status` | Был ли запрос успешен. 1 - да. |
| `id` | Идентификатор анекдота в базе. |
| `anek` | Сам текст анекдота. |
| `source` | Источник из которого был взят анекдот. |
| `s_id` | Идентификатор анекдота в источнике. |
| `views` | Количество просмотров анекдота. |
| `tags` | Массив тегов анекдота. |


### <a name="BAneks-tag"></a> [GET] /tag/:tag
Случайный анекдот категории Б с тегом `tag`.

*Структура ответа:*
```json
{
   "status" : number,
   "id"     : number,
   "anek"   : string,
   "source" : string,
   "s_id"   : string,
   "views"  : number,
   "tags"   : string[]
}
```

| Поле | Описание |
| ---- | -------- |
| `status` | Был ли запрос успешен. 1 - да. |
| `id` | Идентификатор анекдота в базе. |
| `anek` | Сам текст анекдота. |
| `source` | Источник, из которого был взят анекдот. |
| `s_id` | Идентификатор анекдота в источнике. |
| `views` | Количество просмотров анекдота. |
| `tags` | Массив тегов анекдота. |


### <a name="BAneks-id"></a> [GET] /id/:id
Анекдот категории Б с идентификатором `id`.

*Структура ответа:*
```json
{
   "status" : number,
   "id"     : number,
   "anek"   : string,
   "source" : string,
   "s_id"   : string,
   "views"  : number,
   "tags"   : string[]
}
```

| Поле | Описание |
| ---- | -------- |
| `status` | Был ли запрос успешен. 1 - да. |
| `id` | Идентификатор анекдота в базе. |
| `anek` | Сам текст анекдота. |
| `source` | Источник из которого был взят анекдот. |
| `s_id` | Идентификатор анекдота в источнике. |
| `views` | Количество просмотров анекдота. |
| `tags` | Массив тегов анекдота. |


### <a name="BAneks-tags"></a> [GET] /tags
Список всех действительных тегов.

*Структура ответа:*
```json
{
   "status" : number,
   "tags"   : string[]
}
```

| Поле | Описание |
| ---- | -------- |
| `status` | Был ли запрос успешен. 1 - да. |
| `tags` | Массив тегов. |
