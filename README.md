# Кроки для налаштування середовища розробки та компілятора TypeScript

## 1. Створення репозиторію на GitHub:

Створіть новий репозиторій на GitHub і назвіть його 'goit-typescript-hw-01'.

```
git init
git remote add origin https://github.com/your-username/goit-typescript-hw-01.git
git add .
git commit -m "Ініціалізація репозиторію"
git push -u origin master
```

## 2. Налаштування середовища розробки:
Виконайте кроки для налаштування середовища розробки з теми 1.3 “Встановлення та налаштування середовища розробки”.

## 3. Налаштування компілятора TypeScript:
Встановіть TypeScript, якщо ще цього не зробили:

```

npm install -g typescript
tsc --init
npm init -y
```


Створіть файл tsconfig.json та встановіть необхідні параметри:

```
{
  "compilerOptions": {
    "rootDir": "./src",
    "outDir": "./dist",
    "allowJs": false,
    "allowSyntheticDefaultImports": true,
    "emitDecoratorMetadata": true,
    "esModuleInterop": true,
    "experimentalDecorators": true,
    "lib": ["dom", "ES2021"],
    "module": "es2020",
    "moduleResolution": "node",
    "preserveConstEnums": true,
    "skipLibCheck": true,
    "strictNullChecks": true,
    "target": "es2019",
    "sourceMap": true
  },
  "include": ["**/*.ts"]
}
```
```
npm i --save-dev @web/dev-server
```

# 4. Перейдемо до файлу package.json, де нам потрібно додати команду start:
```
{
  "name": "courses_ts",
  "version": "1.0.0",
  "description": "",
  "scripts": {
    "start": "web-dev-server --node-resolve --open --watch"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "@web/dev-server": "^0.2.1"
  }
}

npm start
tsc -w
```
# 5. Опціональне завдання: Встановлення source maps:
Додайте або перевірте, що опція sourceMap встановлена в true у файлі tsconfig.json.

```
{
  "compilerOptions": {
    "sourceMap": true
  }
}
```

