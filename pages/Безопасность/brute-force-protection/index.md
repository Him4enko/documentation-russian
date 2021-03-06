# Защита от Brute Force
<!-- position: 2 -->

## Что такое Brute Forceы?
метод угадывания пароля (или ключа, используемого для шифрования), предполагающий систематический перебор всех возможных комбинаций символов до тех пор, пока не будет найдена правильная комбинация. 

## Как это работает?
Bludit по стандарту включает данную функцию, она позволяет в какой-то мере обезопасить себя от взлома.

Для каждой неудачи входа в систему Blue IT добавляет IP пользователя, который не прошел проверку подлинности, в черный список. Когда пользователь терпит неудачу в течение нескольких раз, плюс он блокирует нарушающий IP-адрес на определенный период времени, и пользователь не может войти в систему, пока срок действия блока не истечет.

## Классы и объекты
Существует объект, который вызывает переменную `$security`,а класс объекта - `/bl-kernel/security.class.php`. Переменные внутри класса:

<pre><code data-language="php">
private $dbFields = array(
    'minutesBlocked'=>5,
    'numberFailuresAllowed'=>10,
    'blackList'=>array()
);
</code></pre>

- `minutesBlocked`: Время на сколько блокируется IP адрес.
- `numberFailuresAllowed`: Количество неудачных попыток для блокировок.
- `blackList`: Список заблокированных IP адресов

<div class="note">
<div class="title">Примечание</div>
Вы можете изменить знчения этих переменных.
</div>