| id тест-кейса | Название тест-кейса                                           | Предусловия                                                                                   | Шаги                                                                                                                             | ОР                                                                                      | Окружение                                              |
| ------------- | ------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| 1             | Вход в аккаунт<br>(Интеграция)                                | 1\. Открыть страницу почтового клиента                                                        | 1\. Ввести валидные данные<br>2\. Нажать кнопку войти                                                                            | Пользователь попадает на главную страницу                                               | Яндекс браузер<br>24.1.0.2570                          |
| 2             | Неотправленное письмо появляется в черновиках<br>(Интеграция) | 1\. Открыть страницу почтового клиента<br>2\. Войти в аккаунт<br>3\. Нажать кнопку "написать" | 1\. Заполнить поле "Кому" любым email<br>2\. Заполнить тело письма любым текстом<br>3\. Закрыть окно или перейти в другой раздел | Письмо появится в разделе "Черновики"                                                   | Яндекс браузер<br>24.1.0.2570                          |
| 3             | Отправка письма<br>(смоук)                                    | 1\. Открыть страницу почтового клиента<br>2\. Войти в аккаунт<br>3\. Нажать кнопку "написать" | 1\. Заполнить поле "Кому" валидным email<br>2\. Заполнить тело письма любым текстом<br>3\. Нажать кнопку "Отправить"             | Письмо отправится адресату и появится в разделе "Отправленные"                          | Яндекс браузер<br>24.1.0.2570                          |
| 4             | Выход из аккаунта<br>(смоук)                                  | 1\. Открыть страницу почтового клиента<br>2\. Войти в аккаунт                                 | 1.Нажать кнопку "Выйти"                                                                                                          | Переход на страницу авторизации                                                         | Яндекс браузер<br>24.1.0.2570                          |
| 5             | Исправление ошибки с удалением письма<br>(ре-тест)            | 1\. Открыть страницу почтового клиента<br>2\. Войти в аккаунт                                 | 1.Перейти в раздел "Входящие"<br>2\. Удалить любое письмо                                                                        | Удаленное письмо не появляется в разделе "Входящие", а появляется в разделе "Удаленные" | Яндекс браузер<br>24.1.0.2570                          |
| 6             | Работоспособность в мобильном браузере<br>(нефункциональное)  | 1\. Открыть страницу почтового клиента на мобильном устройстве<br>                            | 1\. Войти в аккаунт                                                                                                              | Приложение работает корректно                                                           | Android 12<br>Mi note 10 lite<br>Chrome 121.0.6167.164 |


------------------------------------------------------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------------------------------------------------


| Необходимо ли провести регрессионное тестирование приложения электронной почты в случае если добавлен раздел “Спам” |
| ------------------------------------------------------------------------------------------------------------------- |
| Да, добавление нового раздела может повлиять на работу других разделов и связанных функций.                         |

| Необходимо ли провести регрессионное тестирование приложения электронной почты в случае если раздел “Удаленные” переименован в раздел “Корзина” |
| ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Да, переименование раздела может повлиять на его взаимодействие с другими разделами и функциями, если был затронут код. Можно обойтись дымовым. |

| Необходимо ли провести регрессионное тестирование приложения электронной почты в случае если на «Странице входа» устранен ранее обнаруженный дефект |
| --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Для этих целей используется ре-тест                                                                                                                 |


------------------------------------------------------------------------------------------------------------------------------------------------------------------


| Какой вид тестирования желательно провести в первую очередь на новом билде(релизе) приложения?             |
| ---------------------------------------------------------------------------------------------------------- |
| В первую очередь проводится дымовое тестирование, чтобы убедиться, что основные функции работают нормально |

------------------------------------------------------------------------------------------------------------------------------------------------------------------

| В результате добавления раздела “Черновик” перестала корректно работать кнопка “Удалить письмо”. Какой вид тестирования позволит обнаружить нам данный дефект? |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Регрессионное тестирование                                                                                                                                     |
