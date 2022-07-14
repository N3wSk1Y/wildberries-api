# Управление пользователями

Получение пользователей

```
GET http://89.223.65.34:3000/users
```

Удаление пользователя
```
DELETE http://89.223.65.34:3000/users?userid={ID ПОЛЬЗОВАТЕЛЯ}
```

Добавление пользователя
```
POST http://89.223.65.34:3000/users?api_key={КЛЮЧ API WB}&name={ИМЯ ПОЛЬЗОВАТЕЛЯ}&surname={ФАМИЛИЯ ПОЛЬЗОВАТЕЛЯ}
```

Блокировка пользователя
```
LOCK http://89.223.65.34:3000/users?userid={ID ПОЛЬЗОВАТЕЛЯ}
```

Разблокировка пользователя
```
UNLOCK http://89.223.65.34:3000/users?userid={ID ПОЛЬЗОВАТЕЛЯ}
```

Изменение пользователей

Доп. параметры:

`name`, `surname`, `api_key` - изменение одного или нескольких свойств пользователя
```
PUT http://89.223.65.34:3000/users%userid={ID ПОЛЬЗОВАТЕЛЯ}
```

# Управление отчетами

Панель автообновления отчетов - http://89.223.65.34:3000/

Получение отчетов из БД

Доп. параметры:

`dateFrom` и `dateTo` - задать временной диапазон вывода отчетов (формат: 2022-05-30)
```
GET http://89.223.65.34:3000/reports
```

Обновление отчетов в БД
```
POST http://89.223.65.34:3000/reports?api_key={API Ключ}
```
