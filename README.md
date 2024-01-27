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
Copy code
npm install -g typescript
```
Створіть файл tsconfig.json та встановіть необхідні параметри:

```
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true,
    "esModuleInterop": true,
    "sourceMap": true
  }
}
```
# 4. Опціональне завдання: Встановлення source maps:
Додайте або перевірте, що опція sourceMap встановлена в true у файлі tsconfig.json.

```
{
  "compilerOptions": {
    "sourceMap": true
  }
}
```
# 5. Відправлення посилання для перевірки:
Відправте посилання на свій репозиторій ментору для перевірки завдання.

```
git remote add upstream https://github.com/mentor-username/goit-typescript-hw-01.git
git push -u upstream master
```
Завершивши ці кроки, ваше середовище розробки та компілятор TypeScript повинні бути налаштовані та готові для використання.
