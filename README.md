# Базові типи

## Завдання 1

Є наступний JavaScript код:

```ts
const age = 50;
const name = "Max";
const toggle = true;
const empty = null;
const callback = (a) => {
  return 100 + a;
};
```

Перетворіть цей код на TypeScript, вказавши відповідні типи для всіх змінних.

## Завдання 2

У вас є наступний JavaScript масив:

```ts
let person = ["Max", 21];
```

Як переписати його в TypeScript, використовуючи концепцію кортежів, щоб гарантувати, що перший елемент завжди буде рядком, а другий числом?

## Завдання 3

Створіть змінну, яка може містити або `рядок`, або `число` (union type)?
Також, оголосіть змінну, яка може містити `лише одне` з двох можливих рядкових значень: '`enable`' або '`disable`' (literal type).

## Завдання 4

У вас є такі функції JavaScript:

```ts
function showMessage(message) {
  console.log(message);
}

function calc(num1, num2) {
  return num1 + num2;
}

function customError() {
  throw new Error("Error");
}
```

Як ви вкажете типи для аргументів і значень цих функцій, що повертаються?

## Завдання 5

Типізуйте функцію `isWeekend` яка приймає день тижня з `enumDayOfWeek` і повертає `boolean` значення, що вказує, чи це день робочий чи вихідний.

```ts
enum DayOfWeek {
  Monday,
  Tuesday,
  Wednesday,
  Thursday,
  Friday,
  Saturday,
  Sunday,
}

const isWeekend = (day) => {};
```

## Завдання 6

Створіть інтерфейс `User` для типізації об'єктів, які містять такі властивості. Зверніть увагу, що адреса є необов'язковою властивістю.

```ts
const mango = {
  name: "Mango",
  age: 30,
  email: "john@example.com",
  address: {
    city: "New York",
    country: "USA",
  },
};

const poly = {
  name: "Mango",
  age: 30,
  email: "john@example.com",
};
```

## Завдання 7

У вас є два об'єкти:

```ts
const page1 = {
  title: "The awesome page",
  likes: 100,
  accounts: ["Max", "Anton", "Nikita"],
  status: "open",
  details: {
    createAt: new Date("2021-01-01"),
    updateAt: new Date("2021-05-01"),
  },
};

const page2 = {
  title: "Python or Js",
  likes: 5,
  accounts: ["Alex"],
  status: "close",
};
```

Створіть новий тип даних, який підходить для цих двох об'єктів.
