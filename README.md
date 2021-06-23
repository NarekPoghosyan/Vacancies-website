# Авторизация пользователя на MERN стэк, сайт вакансии. (React Js, Express Js, MongoDB, Node Js).

<b>Для начало</b> - _npm install_ в папке _Client_ и _npm install_ в главной папке (в корне) _VACANCIES-WEBSITE_. <br />

<b>Для запуска</b> - _npm run dev_ (Сразу запускается и <b>Front-End</b> и <b>Back-End</b>) в главной папке (в корне) _VACANCIES-WEBSITE_. <br />

Во время ввода полей, пожалуйтса обратите внимание на количество символов, который проситься от вас.

Приложение состоит из клиентской и серверной части, где клиент заполняя свои данные, делает регистрацию и все данные сохраняются в базе данных. После этого он может залогиниться. Если он зашел в систему, генерируется Token, который активен 1 час и сохраняется в localStorage. В течении 1 часа не требуется снова залогиниться. При входе в систему отображается вакансии. Можно посмотреть отдельно каждую вакансию. Есть форма, где можно добавить вакансию и кнопка для выхода из системы.  

# Страница регистрации

![Страница регистрации](https://i.imgur.com/ovF9ML3.png "Страница регистрации")

# Страница авторизации

![Страница авторизации](https://i.imgur.com/XqZGQCv.png "Страница авторизации")

# Страница вакансии (Главная страница)

![Страница вакансии (Главная страница)](https://i.imgur.com/p68HXFp.png "Страница вакансии (Главная страница)")

# Страница для добавление вакансии

![Страница для добавление вакансииt](https://i.imgur.com/15Y2nhV.png "Страница для добавление вакансии")

# Отдельная вакансия

![Отдельная вакансия](https://i.imgur.com/eU4rTg2.png "Отдельная вакансия")

## Ради интереса можно взломать систему.
Во-первых, тут я не должен был добавить файл _config_-ов.
Во-вторых, я специально не сохранил Token в базе данных. Во время рендера страницы _LoginPage_ просто проверяется есть ли Token в localStorage и активирован ли он. Я должен был взять этот Token из localStorage и проверить активирован ли он и совподает с Token - ом, который есть в базе данных. Вы можете просто добавить например такой обьект в localStorage и взломать систему. 

{
    token: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2MGI2NTgyN2Q1MGRkYjFhYjBiMTc5MGEiLCJpYXQiOjE2MjI1NzIzNTUsImV4cCI6MTYyMjU3NTk1NX0.tHglAuCH1HwvC5CYKcq5sQ1r6DJXCUSZBB0zG_Wc2-4"
    userId: "60b65827d50ddb1ab0b1790a"
}

## Использовались такие пакеты...

mongoose <br />
jsonwebtoken <br />
bcrypt <br />
express - validator <br />
config <br />
nodemon <br />
concurrently <br />
proxy <br />
react-router-dom <br />
sass <br />

## Автор Нарек Погосян.
