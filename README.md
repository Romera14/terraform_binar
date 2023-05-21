# Домашнее задание к занятию «Инструменты Git» - Паромов Роман
## Цель задания

### В результате выполнения задания вы:

научитесь работать с утилитами Git;
потренируетесь решать типовые задачи, возникающие при работе в команде.
Инструкция к заданию

Склонируйте репозиторий с исходным кодом Terraform.
Создайте файл для ответов на задания в своём репозитории, после выполнения прикрепите ссылку на .md-файл с ответами в личном кабинете.
Любые вопросы по решению задач задавайте в чате учебной группы.
Задание

## В клонированном репозитории:

Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.
```
commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Jun 18 10:29:58 2020 -0400

    Update CHANGELOG.md

diff --git a/CHANGELOG.md b/CHANGELOG.md
index 86d70e3e0d..588d807b17 100644
--- a/CHANGELOG.md
+++ b/CHANGELOG.md
@@ -27,6 +27,7 @@ BUG FIXES:
 * backend/s3: Prefer AWS shared configuration over EC2 metadata credentials by default ([#25134](https://github.com/hashicorp/terraform/issues/25134))
```

Ответьте на вопросы.
Какому тегу соответствует коммит 85024d3?
* ``` tag: v0.12.23 ```
Сколько родителей у коммита b8d720? Напишите их хеши.
* Коммиты ```56cd7859e05c36c06b56d013b55a252d0bb7e158``` и ```9ea88f22fc6269854151c571162c5bcf958bee2b```
Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.
```
commit 33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24)
    v0.12.24
```
```
commit b14b74c4939dcab573326f4e3ee2a62e23e12f89
    [Website] vmc provider links
```
```
commit 3f235065b9347a758efadc92295b540ee0a5e26e
    Update CHANGELOG.md
```
```
commit 6ae64e247b332925b872447e9ce869657281c2bf
    registry: Fix panic when server is unreachable
    
    Non-HTTP errors previously resulted in a panic due to dereferencing the
    resp pointer while it was nil, as part of rendering the error message.
    This commit changes the error message formatting to cope with a nil
    response, and extends test coverage.
    
    Fixes #24384
```
```
commit 5c619ca1baf2e21a155fcdb4c264cc9e24a2a353
    website: Remove links to the getting started guide's old location
    
    Since these links were in the soon-to-be-deprecated 0.11 language section, I
    think we can just remove them without needing to find an equivalent link.
```
```
commit 06275647e2b53d97d4f0a19a0fec11f6d69820b5
    Update CHANGELOG.md
```
```
commit d5f9411f5108260320064349b757f55c09bc4b80
    command: Fix bug when using terraform login on Windows
```
```
commit 4b6d06cc5dcb78af637bbb19c198faff37a066ed
    Update CHANGELOG.md
```
```
commit dd01a35078f040ca984cdd349f18d0b67e486c35
    Update CHANGELOG.md
```
```
commit 225466bc3e5f35baa5d07197bbc079345b77525e
    Cleanup after v0.12.23 release
```
Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...) (вместо троеточия перечислены аргументы).
```
8c928e8358
```
Найдите все коммиты, в которых была изменена функция globalPluginDirs.
* не нашел командами из лекции изменений в файлах plugin.go, command.go, config.go
Кто автор функции synchronizedWriters?
```
Author: Martin Atkins <mart@degeneration.co.uk>
```
В качестве решения ответьте на вопросы и опишите, как были получены эти ответы.
* Ответы были получены с помощью комманд из лекций.
Правила приёма домашнего задания

В личном кабинете отправлена ссылка на .md-файл в вашем репозитории.

Критерии оценки

Зачёт:

выполнены все задания;
ответы даны в развёрнутой форме;
приложены соответствующие скриншоты и файлы проекта;
в выполненных заданиях нет противоречий и нарушения логики.
На доработку:

задание выполнено частично или не выполнено вообще;
в логике выполнения заданий есть противоречия и существенные недостатки.
