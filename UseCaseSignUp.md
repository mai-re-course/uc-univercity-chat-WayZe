# Термины предметной области

Преподаватель.  
Студент.  
Пользователь — преподаватель или студент.  
Мобильное приложение.  
Веб-сайт.  
Приложение — мобильное приложение или веб-сайт.  
База данных.  

# Сценарии использования
## Регистрация пользователя

**Акторы:** пользователь.

**Цель:** пользователь регистрируется в приложении.

**Предусловия:** пользователь зашел на страницу регистрации.

**Сценарий:**
1. Пользователь вводит данные.
2. Пользователь нажимает кнопку "Зарегистрироваться".
3. Приложение отправляет данные серверу.
4. Сервер записывает данные нового пользователя в базу данных.
5. Сервер возвращает код успешной регистрации.
6. Приложение открывает страницу профиля пользователя.

**Результат:**

- Открывается страница профиля пользователя.  
- В базе данных создается новый пользователь . 

**Альтернативные или исключения:** 

1.1. Пользователь нажимает кнопку социальной сети, через которую он хочет зарегистрироваться.  
1.2. Приложение открывает окно авторизации выбранной социальной сети.  
1.3. Пользователь вводит логин и пароль от социальной сети.  
1.4. Приложение отправляет данные на сервер социальной сети.  
1.5. Сервер социальной сети возвращает успешный код регистрации.  
1.6. Переход к шагу 4.  

1.5.1. Сервер социальной сети возвращает код ошибки.  
1.5.2. Приложение выводит пользователю сообщение о ошибки авторизации в социальной сети.  

5.1. Сервер возвращает код ошибки.  
5.2. Приложение выводит пользователю сообщение об ошибке регистрации.  
