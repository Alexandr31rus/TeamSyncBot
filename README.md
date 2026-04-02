## Структура проекта
```
team_sync_bot/
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py          # FastAPI приложение
│   │   ├── database.py      # SQLAlchemy модели, соединение
│   │   ├── crud.py          # операции с БД
│   │   ├── schemas.py       # Pydantic модели
│   │   ├── bot/
│   │   │   ├── __init__.py
│   │   │   ├── bot.py       # aiogram 3 диспетчер
│   │   │   ├── handlers.py  # обработчики сообщений
│   │   │   ├── keyboards.py # клавиатуры
│   │   │   └── states.py    # FSM состояния
│   │   └── routers/
│   │       ├── tasks.py
│   │       └── ideas.py
│   ├── requirements.txt
│   └── .env
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/        # API вызовы к FastAPI
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
├── docker-compose.yml       # для локального запуска с БД
└── README.md
```