Создание полноценного укорачивателя ссылок с использованием только HTML, CSS и JavaScript без серверной части невозможно, так как для укорачивания ссылок требуется сервер, который будет хранить соответствие между оригинальными и сокращёнными URL и перенаправлять пользователей по сокращённым ссылкам.

Однако можно создать упрощённый интерфейс для укорачивателя ссылок, который будет взаимодействовать с уже существующим API укорачивателя ссылок. Например, можно использовать API сервиса bitly.com или других подобных сервисов (для этого потребуется зарегистрироваться и получить API ключ). Для примера возьмем сервис bitly (предполагая, что у вас есть ключ API).

Вот пример такой HTML-страницы с использованием Bootstrap для стилизации и jQuery для упрощения работы с AJAX


В этом примере, когда пользователь вводит URL и нажимает кнопку "Сократить URL", JavaScript (с помощью jQuery) отправляет AJAX-запрос к API Bitly для сокращения URL. В случае успешного ответа от API, сокращенный URL отображается на странице.

Не забудьте заменить 'ВАШ_BITLY_ТОКЕН' на актуальный токен доступа API Bitly.

