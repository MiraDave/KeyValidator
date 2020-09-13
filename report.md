# Отчёт о тестировании KeyValidator

Приложение KeyValidator распространяется в виде файла KeyValidator.class, предназначенного для работы на платформе Java 8+.

13.09.2020 были проведены функциональное тестирование и тестирование установки приложения KeyValidator.

На тестирование затрачено: 7 часов

В результате тестирования выявлены следующие дефекты:

* [Валидный ключ не проходит проверку #1](https://github.com/MiraDave/KeyValidator/issues/1#issue-700586518)

* [Валидный ключ не проходит проверку #2](https://github.com/MiraDave/KeyValidator/issues/2#issue-700587882)

* [Валидный ключ не проходит проверку #3](https://github.com/MiraDave/KeyValidator/issues/3)

* [Невалидный ключ проходит проверку](https://github.com/MiraDave/KeyValidator/issues/4)

В процессе тестирования использовались следующие артефакты:

* файл [KeyValidator.class](intro/user-manual.md)

* файл [.gitignore](.gitignore)

В качестве тестовых данных использовались данные [Руководство использования KeyValidator](intro/user-manual.md):

При вводе валидных ключей должно появится "OK", при вводе невалидных ключей - "FAIL"

Валидные ключи:
* 00000000-0000-0000-0000-000000000000
* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
* 80b427f8-92cd-3aae-ba04-3927fbe17c6
* b295bc63-9f03-3b4b-af80-969b39f8c262
* 387eedc6-12e9-3b32-9881-63b6b5e85317
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180

Невалидные ключи:
* 00000000-0000-0000-0000-000000000001
* 18252235-78e0-44a5-8720-556f0c7da17a
* e66075b6-ddad-445e-baf6-161b3289522b
* b6d53250-f07e-4352-a293-6102ddf7f1ca
* c2bc778a-1cb9-46c6-b435-0489649d2a42
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

Тестирование производилось в следующем окружении:

* Windows 10 x64
* Java "11.0.8" 2020-07-14