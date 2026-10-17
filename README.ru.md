# Pizza Service: frontend (Tel-Ran, 2023)

[English](README.md) | [Русский](README.ru.md)

Frontend Pizza Service — моего дипломного проекта в Tel-Ran. Я самостоятельно разработал интерфейс на React: список кафе, страницы добавления и изменения кафе, каталог пиццы.

REST API предоставляет [бэкенд на Java](https://github.com/ivan-zamula/pizza-service-backend-2023-tel-ran).

## Интерфейс

![Список кафе Pizza Service с поиском и действиями управления](docs/images/pizza-service-cafe-list.jpeg)

Список кафе в React-интерфейсе, который я самостоятельно разработал для дипломного проекта в Tel-Ran.

## Стек и структура

React, React Router, Axios, Bootstrap, Reactstrap и Material UI. Для сборки используется `react-scripts` 5.

| Путь | Содержимое |
| --- | --- |
| [frontend/src/App.js](frontend/src/App.js) | Маршруты приложения |
| [frontend/src/components/cafe](frontend/src/components/cafe) | Страницы кафе |
| [frontend/src/components/pizza](frontend/src/components/pizza) | Список пиццы |
| [frontend/src/services](frontend/src/services) | Axios-клиенты для бэкенда |
| [frontend/package.json](frontend/package.json) | Зависимости и команды npm |

## Локальный запуск

Установите Node.js и npm. Перед работой с интерфейсом запустите парный бэкенд на `http://localhost:8080`.

```bash
git clone https://github.com/ivan-zamula/pizza-service-frontend-2023-tel-ran.git
cd pizza-service-frontend-2023-tel-ran
```

```bash
cd frontend
npm ci
npm start
```

Откройте [http://localhost:3000](http://localhost:3000). Адреса API заданы в [CafeService.js](frontend/src/services/CafeService.js) и [PizzaService.js](frontend/src/services/PizzaService.js).

Из каталога `frontend/` команда `npm run build` создает сборку в `build/`, а `npm test` запускает тесты. Параметр `homepage` в `package.json` задает базовый путь к ресурсам опубликованной сборки.
