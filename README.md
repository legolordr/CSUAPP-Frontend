# CSUAPP-Frontend
**Пробничек репозитория**  
# Документация

В репозитории используется FSD архитектура - организация кода по бизнес - фичам.
Такой подход ускоряет параллельную разработку, упрощает тестируемость и отлично синхронизируется с микросервисами.

## Обзор 
- **`public`** - папка со статическими файлами/файлы которые не проходят обработку перед попаданием в корень приложения
- **`src`** - исходный код приложения
- **`src/app`** - инициализация приложения, тут лежит конфигурация маршрутизации **`routes`**, глобальные сторы уровня приложения **`stores`**, точка входа `index.ts`, корневой Svelte `app.svelte`,ну и стили `app.css`
- **`src/features`** - слой фич, каждая фича - изолированный модуль с полной бизнес - логикой.У каждой фичи присутствуют следующее папки: **`components`** -  UI - компоненты на Svelte; **`services`** - бизнес логика; **`api`** - api запросы; `index.ts` - публичный API.
- **`src/pages`** - каждая папка это страница приложения.
- **`src/shared`** - переиспользуемый код, который ничего не знает о бизнес логике. Базовая UI - система, базовый http клиент, общие сторы, общие TS типы и тп.

Created with https://www.readmecodegen.com  
```
📁 CSUAPP/
├── 📁 public/
├── 📁 src/
│   ├── 📁 app/
│   │   ├── 📁 routers/
│   │   ├── 📁 stores/
│   │   ├── 🟦 index.ts
│   │   ├── 📄 App.svelte
│   │   └── 🎨 App.css
│   ├── 📁 features/
│   │   ├── 📁 food/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   ├── 📁 navigation/
│   │   │   ├── 📁 Threlte/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   ├── 📁 searchTeacher/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   ├── 📁 schedule/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   ├── 📁 admin/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   ├── 📁 auth/
│   │   │   ├── 📁 components/
│   │   │   ├── 📁 services/
│   │   │   ├── 📁 api/
│   │   │   └── 🟦 index.ts
│   │   └── 📁 profile/
│   │       ├── 📁 components/
│   │       ├── 📁 services/
│   │       ├── 📁 api/
│   │       └── 🟦 index.ts
│   ├── 📁 pages/
│   │   ├── 📁 admin/
│   │   ├── 📁 food/
│   │   ├── 📁 home/
│   │   ├── 📁 im/
│   │   ├── 📁 login/
│   │   ├── 📁 navigation/
│   │   ├── 📁 profile/
│   │   ├── 📁 register/
│   │   ├── 📁 schedule/
│   │   └── 📁 search-teacher/
│   └── 📁 shared/
│       ├── 📁 api/
│       ├── 📁 config/
│       ├── 📁 lib/
│       ├── 📁 stores/
│       ├── 📁 types/
│       ├── 📁 ui/
│       └── 📁 ws/
├── 📄 .gitignore
└── 📄 README.md

```
