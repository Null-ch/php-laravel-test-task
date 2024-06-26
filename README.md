## Описание
Тестовые задания предлагаемые на вакансии PHP разработчику. Содержатся задания по PHP, Laravel, Bitrix <br>
Отдельное спасибо участникам нашего микро сообщества для джунов <a href="https://laravel.com" target="_blank">Junior PHP (Laravel)</a><br>

<details>
<summary>## Тестовые задания "Нативный PHP"</summary><br>
<details>
<summary>Первое задание</summary>
<h5>Задание:</h5>
Товары со склада уезжают в магазин каждый день, количество товаров на отправку в магазин формируется из предзаказов. <br>
Кол-во предзаказов варьируется. Перед тем, как отправить товары в магазин, специально обученный сотрудник (далее СОС) наклеивает ценники на товар. Цена - это себестоимость товара с 30% наценкой.<br>
Вводные: Начиная с 13 января 2021 года товар “Левый носок” предзаказывают каждый день, кол-во ежедневных предзаказов совпадает с последовательностью чисел Фибоначчи. <br>
Необходимо разработать систему, которая будет помогать СОС в его работе, а именно каждый день говорить, какие ценники клеить на товар, при условии что на всех ценниках в рамках одного дня должна быть одинаковая цена:<br>
<h5>Требования:</h5><br>
 - Веб страница с инпут полем, кнопкой применить и секцией с информацией.<br>
 - Инпут поле с возможностью выбора даты (для эмуляции сменяемости дней)<br>
 - На день, который выбран в инпут поле, нужно отобразить в секции с информацией: остаток на складе и текущую цену товара.<br>
 - Обработать возможные ошибки ввода (Не валидная дата, неверная дата), для каждого типа ошибок должно отображаться свое сообщение<br>
</details>
<details>

<summary>Второе задание</summary>
<h5>Задание:</h5>
Написать формы регистрации, авторизации, страницу профиля:<br>
<h5>Требования:</h5>
В форме регистрации пользователь должен указать Имя, телефон, почту, пароль и повтор пароля.<br>
Почта, логин и телефон должны быть уникальны и если такие в базе уже есть - уведомлять пользователя об этом.<br>
Пароли в обоих полях должны совпадать, иначе уведомлять пользователя об этом.<br>
Авторизация возможна по телефону или email (в одном поле) и паролю, необходимо добавить Google reCAPTCHA при авторизации.<br>
Сделать страницу, к которой только авторизованные пользователи имеют доступ. Неавторизованные пользователи должны перенаправляться на главную страницу. На этой странице пользователи могут менять свою личную информацию (имя, телефон, почта, пароль).<br>
</details>
<details>

<summary>Третье задание "Сервис-агрегатор для проведения фиктивных опросов"</summary>
<h5>Задание:</h5>
<h5>Необходим сервис, который предоставит функционал управления фиктивными опросами (с заранее определенным количеством голосов). Пользователь сервиса может зайти на публичную часть программы, зарегистрироваться и создать опросы с определенным числом ответов в формате:</h5>
Вопрос:<br>
1. Ответ 1<br>
2. Ответ 2<br>
3. ...<br>
...<br>
n. ...<br>

<h5>Функционал:</h5>
1. Аутентификация на сервисе:<br>
   - Страница регистрации<br>
   - Страница входа<br>
   - Разлогин<br>
2. Для пользователя достаточно ввести только email и пароль.<br>
3. Аутентифицированный пользователь попадает в личный кабинет.<br>

<h5>Личный кабинет:</h5>
- Содержит раздел с списком собственных опросов.<br>
- Сортировка списка по "дате создания", "заголовку", "статусу".<br>
- CRUD для управления опросами.<br>
- Каждый опрос содержит:<br>
  1. Текст вопроса (заголовок).<br>
  2. Любое количество ответов.<br>
  3. Количество голосов для каждого ответа.<br>
  4. Статус "черновик" или "опубликован".<br>

<h5>Конечный пользователь, использующий сервис, должен получить доступ к API для получения данных опубликованного случайного опроса из своего списка. Данные должны включать:</h5>
- Заголовок.<br>
- Пункты ответов с количеством голосов для каждого.<br>

API тестируется с использованием Postman.

<h5>Требования к реализации:</h5>
1. Реализация на чистом PHP без использования фреймворков.<br>
2. Можно использовать библиотеки на ваш выбор.<br>
3. Приложение должно быть написано в стиле ООП.<br>
4. Используйте MVC модель для организации работы программы.<br>
5. Необходима простая архитектура, следуйте YAGNI.<br>
6. Принцип уникальности.<br>
7. Верстка на bootstrap, особых дизайнерских требований нет.<br>

<h5>После выполнения задания необходимо:</h5>
1. Предоставить ссылку на git-репозиторий вашей работы.<br>
2. Предоставить минимально необходимую документацию в удобном для чтения виде с описанием работы API.<br>
3. Развернуть на любом бесплатном хостинге для просмотра результата.<br>

</details>
<details>
<summary>Четвертое задание</summary>
<h5>Задание:</h5>
Создайте две простых формы
<h5>Требования:</h5>
 * Используйте для проекта PHP8 / bootstrap / js / css / html / GIT<br>
 * Кодировка (файлы/контент) только UTF-8 / EOL только LF / EOF только LF!<br>
<br>
В корне проекта создайте:<br>
 * Директории /assets/js/ и /assets/css/ для соответствующих файлов<br>
 * Файл - /index.php – редирект на /step/1/index.html<br>
<br>
Создайте две простых формы:<br>
Форма №1 (/step/1/index.html и обработчик /step/1/action.php)<br>

  На форме №1 расположено два поля ввода:<br>
1. Введите имя нового ЛК (текстовое поле (с подсказкой ниже «Имя должно состоять из английских прописных букв от a до z, может содержать знак минус "-"»))<br>
2. Введите название клиента на русском (текстовое поле)<br>

  Кнопка «Далее»<br>
При нажатии кнопки «Далее» пишем файл:<br>
/files/step/(данные из поля «Введите имя нового ЛК»)/step_1.txt<br>
  На фс с содержимым полей в формате:<br>
 * «Введите имя нового ЛК»|«Введите название клиента на русском»<br>
Так же передайте данные из поля «Введите имя нового ЛК» на форму №2.<br>
<br>
Форма №2 (/step/2/index.html и обработчик /step/2/action.php)<br>
На форме №2 расположено 2 поля в блоке:<br>
1. Login(Электронная почта);<br>
2. Фамилия Имя.<br>
В блоке должен присутствовать знак «+» - для добавления блока, знак «-» - для удаления блока.<br>
При нажатии кнопки «Готово» пишем файл:<br>
/files/step/(данные из поля «Введите имя нового ЛК» формы №1)/step_2.txt<br>
на фс с содержимым полей всех блоков в формате:<br>
 * «Введите имя нового ЛК» формы №1|«Login(Электронная почта)»| «Фамилия Имя»<br>
 * «Введите имя нового ЛК» формы №1|«Login(Электронная почта)»| «Фамилия Имя»<br>

</details>

<details>
<summary>Пятое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/0c8af2ad-e7cc-4c0c-a799-ec343857e965">
</details>
</details>
<br>

<details>
<summary>## Тестовые задания "Laravel"</summary><br>

<details>
<summary>Первое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/f159f307-0378-4a78-8505-dcd9a87580cb">

</details>

<details>
<summary>Второе задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/20a5a49e-4b0d-49fb-82fa-680d71717f58">
</details>

<details>
<summary>Третье задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/ac716c75-3d7f-4040-8d8a-f2b246005867">

</details>

<details>
<summary>Четвертое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/663b0e4d-9b40-40d5-af4c-306e5cf99e9f">
</details>

<details>
<summary>Пятое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/6f566917-61c4-401f-8d97-f7e7c95c7877">
</details>

<details>
<summary>Шестое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/9529f702-a1dd-4b92-aad5-14bb574180e0">
</details>

<details>
<summary>Седьмое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/8d0230ad-be49-4b31-9683-4e745224abb6">
<h5>Пример реализации:</h5><br>
https://github.com/Null-ch/Jetmix_test_task
</details>

<details>
<summary>Восьмое задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/fd00ef23-e85d-44cf-9cc1-1d8e22bd7f41">
<h5>Пример реализации:</h5><br>
https://github.com/Null-ch/Dataloft_test28_task_API
</details>
</details><br>

<details>
<summary>## Тестовые задания Bitrix</summary><br>
  
<details>
  <summary>Первое задание</summary>
  <h5>Задание:</h5>
  <img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/eb233db6-5db9-456d-99b0-4dd8b72dab02">
ДОКУМЕНТАЦИЯ к ТЗ
Требования к заданию №5
Задание должно быть выполнено с использованием регулярного выражения.<br>
Важно предусмотреть безопасность передаваемых данных.<br>
Гуглить можно, но запрещено использовать готовые примеры.<br>
Документация к заданию №2,4 https://dev.1c-bitrix.ru/api_help/iblock/functions/getiblockelementlist.php <br>
Документация к заданию №3 https://dev.1c-bitrix.ru/api_help/main/reference/cuser/getlist.php<br>
Документация к заданию №3,4 https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=43&LESSON_ID=2894&LESSON_PATH=3913.3435.4777.2894<br>
</details>

<details>
<summary>Второе задание</summary>
<h5>Задание:</h5>
<img src="https://github.com/Null-ch/php-laravel-test-task/assets/65172872/f097787e-b0e3-4c45-86e3-fd85e75f9c17">

Примечание
По итогу работы сделать резервное копирование через админку, залить полученный бэкап в облако и отправить на почту ссылку с админскими доступами.
Дополнительные материалы
Как развернуть битрикс: [линк](https://docs.google.com/document/d/19RuvvkygrTdqiNzXZ7N6CLzQMofNjf5tKvwvSm5ndts/edit?usp=sharing) <br>
 Документация по компонентам: [линк](https://dev.1c-bitrix.ru/user_help/components/content/index.php) <br>
 Видео: [линк](https://www.youtube.com/channel/UCqwGlnyM-tro3ArkhiVyIxg/videos) <br>
</details>
</details>
