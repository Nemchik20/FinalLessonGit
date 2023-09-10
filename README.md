# FinalLessonGit
## Задание SkillFactory
- Привет мир 
- Это тема Git 
- Система контроля версиями - это система, записывающая изменение в файл или набор файлов в течение времени и позволяющая позже вернуться к определеной версии.

# Типы систем -> Локальная СКВ, Централизованная СКВ, Распределенная СКВ.
- Локальные СКВ -> хранят информацию об всех изменениях внесеных в файлы, в базе данных которая так же хранится на локальном компьюторе. Основываясь на этих данных система контроля версиями воссоздает нужную версию (актуальную на определенный момент времени) в локальный СКВ обычно храниться список изменение, внесенных в файлы.
- Достоинства 
- 1. Возможность востановление данных из определенных версий (Точно определяются по времени записи)
- 2	. Высокая скорость востановление (База данных четко структурирована, сетевая задержка отсутсвует, так как данные хранятся непосредственно на компьюторе)
- Недостатки 
- 1. Возможность потери данных при физической поломке оборудывания
- 2. Сложность разработки. Одновременно изменение в определенный файл могут быть внесены только одним пользователем

# Централезованое СКВ 
- В централизованных системах появляется удаленных репозиторий, который находиться на сервере в Сети, Проекты над которыми работают разрабочики, импортируются в локальный репозиторий. Таким образом, появляется возможность работы над одними и  теме же файлами одновременно.
- Достоинства 
- 1. Возможность распределенной разработки
- 2. Полный контроль администратора над процессом разработки с помощью выдачи конкретных прав для пользователей 
- Недостатки 
- 1. Единная точка отказа который является центральный сервер. Если сервер выйдет из строя никто не то никто не сможет ни взаиможействовать друг с другом ни сохранить изменение в файл с которым работает. А вслучае когда жесткий диск, будет поврежден а резерных копиий не будет, вся история проекта (за исключением еденичных списков репозитория, которые сохранились на локальных машинах) может быть утеряна.

# Распределенная СКВ
- В распределенных системах не сущестует Центрального репозиторя, все коппии создаются равными. Что резко отличает от централизованных СКВ, где работа основана на добавление и извлечение из централизованного репозитория. Это означает, что разрабочики могут обмениваться изменениями друг с другом перед обьядинениями своих в официальную сеть 
- Достоинства 
- 1. Разрабочики могут вносить свои изменение в локальную копию репозитория без ведома других репозиториев 
- 2. Можно вносить фиксацию изменение без подключение к интернету, разрабочики могут работать локально в автономном режиме пока не будут готовы поделиться своей работой с другими
- 3. При отказе одного из серверов через который разрабочики обмениваются данными любой клиентский репозиторий может быть скопирован на другой сервер для продолжение работы. каждый репозиторий является полной коппией всех данных с помощью которых можно востановить потеряные или поврежденную информацию о проекте

- Git - это распределенная система контроля версий. Git отличается от других СКВ подходом с работе с данными 

- Синтаксис MarkDown 
# Заголовок
## Заголовок 

*Текст использовается для выделение курсивом*
**Текст использовается для выделение жирным**
* текст Использовается для обозначение элемента не нумерованого списка  
1.текст  используется для обозначение элемента нумерованого списка
[Назвение](Сыллка)


# Основные операции в GIt 
## Commit
*Commit - Это состояние репозитория в определенный момент времени. Иммено к коммиту мы можем вовзращатся, чтобы посмотреть состояние обьектов в какое-то время

