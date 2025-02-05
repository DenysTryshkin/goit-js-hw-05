Time flies so fast, doesn't it?

After studying this week's materials, you:

*   Understand how callback functions and arrow functions work
*   Can apply these functions in practice
*   Know how to work with an array of objects
*   Are familiar with array methods such as: `forEach`, `map`, `flatMap`, `filter`, `find`, `every`, `some`, `reduce`, and `toSorted`
*   Can set up custom sorting for numbers and strings
*   Know how to use array methods in chains

Now, let's move on to practice!  
You have four tasks ahead that require you to use the array methods you've learned.

* * *

### Homework: Topic 8 - Array Iteration Methods

1.  **Create a repository** called `goit-js-hw-05` and clone it to your computer.
2.  Inside the `goit-js-hw-05` folder, create the project structure as shown in the diagram below.

**Important!**  
The names of files and folders, as well as their nesting structure, must match the specified scheme. Otherwise, your work will not be accepted.

![Project structure](https://s3.eu-north-1.amazonaws.com/lms.goit.files/7ef8973c-cfea-416c-8232-05c93b5d033cFrame%2048672%20%282%29.jpg)

3.  Read each task carefully and complete it in the corresponding file.
4.  Ensure that your code is formatted using `Prettier`, and that no errors or warnings appear in the console when opening the live task page.
5.  Submit the homework for review.

* * *

### Submission Format:

Your homework submission must include two links:

*   A link to the repository with your code
*   A live page link on `GitHub Pages`

Additionally, attach the repository file in `.zip` format.

☝ **IMPORTANT**  
Review the **[Instructions for uploading your working file from the repository to GitHub](https://drive.google.com/file/d/1UBw9IkvLmk4hO73ji1ScNkj3_H_vKNvT/view?usp=sharing)**

* * *

### Evaluation Criteria:

*   Pass / Fail

* * *

## Task 1: User Names

Complete this task in the file `task-1.js`.

Write an arrow function `getUserNames(users)` that takes one parameter:

*   `users` – an array of user objects.

The function should return an array of all user names (property `name`) from the `users` array.

Use the following code to test your function. The results of its calls will be displayed in the console.


`console.log(   getUserNames([     { name: "Moore Hensley", email: "moorehensley@indexia.com", balance: 2811 },     { name: "Sharlene Bush", email: "sharlenebush@tubesys.com", balance: 3821 },     { name: "Ross Vazquez", email: "rossvazquez@xinware.com", balance: 3793 },     { name: "Elma Head", email: "elmahead@omatom.com", balance: 2278 },     { name: "Carey Barr", email: "careybarr@nurali.com", balance: 3951 },     { name: "Blackburn Dotson", email: "blackburndotson@furnigeer.com", balance: 1498 },     { name: "Sheree Anthony", email: "shereeanthony@kog.com", balance: 2764 },   ]) );  // ["Moore Hensley", "Sharlene Bush", "Ross Vazquez", "Elma Head", "Carey Barr", "Blackburn Dotson", "Sheree Anthony"]`

Leave this code for the mentor's review.

* * *

## Task 2: Users with a Friend

Complete this task in the file `task-2.js`.

Write an arrow function `getUsersWithFriend(users, friendName)` that takes two parameters:

*   `users` – an array of user objects.
*   `friendName` – the name of the friend to search for.

The function should return an array of all users from `users` who have a friend with the name `friendName`.  
Friends of each user are stored in the `friends` property. If no users have such a friend, the function should return an empty array.

### Hints:

*   The `filter()` method can be used to create a new array with elements that meet a specific condition.
*   Use the `includes()` method to check if the `friends` array contains `friendName`.

Use the following code to test your function:


`const allUsers = [   { name: "Moore Hensley", friends: ["Sharron Pace"] },   { name: "Sharlene Bush", friends: ["Briana Decker", "Sharron Pace"] },   { name: "Ross Vazquez", friends: ["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"] },   { name: "Elma Head", friends: ["Goldie Gentry", "Aisha Tran"] },   { name: "Carey Barr", friends: ["Jordan Sampson", "Eddie Strong"] },   { name: "Blackburn Dotson", friends: ["Jacklyn Lucas", "Linda Chapman"] },   { name: "Sheree Anthony", friends: ["Goldie Gentry", "Briana Decker"] } ];  console.log(getUsersWithFriend(allUsers, "Briana Decker"));  // Expected output: [{ name: "Sharlene Bush", friends: ["Briana Decker", "Sharron Pace"] }, { name: "Sheree Anthony", friends: ["Goldie Gentry", "Briana Decker"] }]  console.log(getUsersWithFriend(allUsers, "Goldie Gentry"));  // Expected output: [{ name: "Elma Head", friends: ["Goldie Gentry", "Aisha Tran"] }, { name: "Sheree Anthony", friends: ["Goldie Gentry", "Briana Decker"] }]  console.log(getUsersWithFriend(allUsers, "Adrian Cross"));  // Expected output: []`

* * *

## Task 3: Sorting by Number of Friends

Complete this task in the file `task-3.js`.

Write an arrow function `sortByDescendingFriendCount(users)` that takes one parameter:

*   `users` – an array of user objects.

The function should return an array of all users, sorted in descending order by the number of their friends (`friends`property).

Use the `toSorted()` method.

* * *

## Task 4: Total Balance by Gender

Write an arrow function `getTotalBalanceByGender(users, gender)` that takes two parameters:

*   `users` – an array of user objects.
*   `gender` – a string representing gender.

The function should use method chaining and return the total balance of users (`balance` property) whose gender (`gender`property) matches the `gender` parameter.

Use the following code to test your function:


`const clients = [   { name: "Moore Hensley", gender: "male", balance: 2811 },   { name: "Sharlene Bush", gender: "female", balance: 3821 },   { name: "Ross Vazquez", gender: "male", balance: 3793 },   { name: "Elma Head", gender: "female", balance: 2278 },   { name: "Carey Barr", gender: "male", balance: 3951 },   { name: "Blackburn Dotson", gender: "male", balance: 1498 },   { name: "Sheree Anthony", gender: "female", balance: 2764 } ];  console.log(getTotalBalanceByGender(clients, "male")); // Expected output: 12053 console.log(getTotalBalanceByGender(clients, "female")); // Expected output: 8863`

* * *

Follow the given instructions to complete and submit your homework successfully. Good luck! 🚀

________________________________

Час так швидко плине, чи не так?

Після вивчення матеріалів цього тижня ти:

*   розумієш принцип роботи колбек-функцій та стрілочних функцій
*   вмієш застосовувати ці функції на практиці
*   знаєш, як працювати з масивом об'єктів
*   знаєш такі методи масивів, як: `forEach`, `map`, `flatMap`, `filter`, `find` і `every`, `some`, `reduce`, `toSorted`
*   вмієш налаштувати свій порядок сортування чисел та рядків
*   знаєш, як використовувати методів масиву у ланцюжках

  

А тепер давай перейдемо до практики!
На тебе чекають 4 задачі, в яких треба використати вивчені методи масивів!

  

**Домашнє завдання Тема 8. Перебераючі методи масивів**

  

*   Створи репозиторій `goit-js-hw-05` та склонюй його собі на комп’ютер.
*   У папці `goit-js-hw-05` створи структуру проєкта, як показано на схемі нижче.

**Зверни увагу!** 
Імена файлів та папок, а також їх структура вкладеності, мають відповідати вказаній схемі. В іншому разі робота не буде прийнята.

  

![](https://s3.eu-north-1.amazonaws.com/lms.goit.files/7ef8973c-cfea-416c-8232-05c93b5d033cFrame%2048672%20%282%29.jpg)

  

  

*   Прочитай кожне завдання і виконай його у відповідному файлі.
*   Переконайся, що код відформатований за допомогою `Prettier`, а в консолі відсутні помилки й попередження під час відкриття живої сторінки завдання
*   Здай домашнє завдання на перевірку

  

**Формат здачі:**

*   Домашня робота містить два посилання: на вихідні файли (посилання на репозиторій з кодом) і живу сторінку на `GitHub Pages`.
*   Прикрiплений файл репозиторію у форматi zip

☝ **ВАЖЛИВО**
Переглянь [**Iнструкцію щодо завантаження робочого файлу з репозиторію на Github**](https://drive.google.com/file/d/1UBw9IkvLmk4hO73ji1ScNkj3_H_vKNvT/view?usp=sharing)

  

**Формат оцінювання:**

*   Залiк / Незалiк

  

  

**Задача 1. Імена користувачів**

  

Виконуй це завдання у файлі `task-1.js`

  

Напиши стрілочну функцію `getUserNames(users)`, яка прийматиме один параметр `users` — масив об’єктів користувачів. Функція має повертати масив імен усіх користувачів (властивість `name`) із масиву `users`.

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її викликів.

  

console.log(
  getUserNames(\[
  {
    name: "Moore Hensley",
    email: "moorehensley@indexia.com",
    balance: 2811
  },
  {
    name: "Sharlene Bush",
    email: "sharlenebush@tubesys.com",
    balance: 3821
  },
  {
    name: "Ross Vazquez",
    email: "rossvazquez@xinware.com",
    balance: 3793
  },
  {
    name: "Elma Head",
    email: "elmahead@omatom.com",
    balance: 2278
  },
  {
    name: "Carey Barr",
    email: "careybarr@nurali.com",
    balance: 3951
  },
  {
    name: "Blackburn Dotson",
    email: "blackburndotson@furnigeer.com",
    balance: 1498
  },
  {
    name: "Sheree Anthony",
    email: "shereeanthony@kog.com",
    balance: 2764
  },
\])
); // \["Moore Hensley", "Sharlene Bush", "Ross Vazquez", "Elma Head", "Carey Barr", "Blackburn Dotson", "Sheree Anthony"\]

  

Залиш цей код для перевірки ментором.

  

**На що буде звертати увагу ментор при перевірці:**

*   Оголошена змінна `getUserNames`
*   Змінній `getUserNames` присвоєна стрілочна функція з параметром `(users)`.
*   Для перебирання параметра `users` використовується метод `map()`
*   Виклик функції із зазначеним масивом користувачів повертає масив `["Moore Hensley", "Sharlene Bush", "Ross Vazquez", "Elma Head", "Carey Barr", "Blackburn Dotson", "Sheree Anthony"]`
*   Виклик функції з випадковими, але валідними аргументами повертає правильне значення

  

  

**Задача 2. Користувачі з другом**

  

Виконуй це завдання у файлі `task-2.js`

  

Напиши стрілочну функцію `getUsersWithFriend(users, friendName)` , яка прийматиме два параметра:

*   перший параметр `users` — масив об’єктів користувачів
*   другий параметр `friendName` — ім’я друга для пошуку.

  

Функція має повертати масив усіх користувачів із масиву `users`, у яких є друг з іменем `friendName`. Друзі кожного користувача зберігаються у властивості `friends`. Якщо користувачів, у яких є такий других немає, то функція має повернути порожній масив.

  

**Поради:**

*   Метод `filter()` можна використовувати для створення нового масиву з елементами, які задовольняють певну умову.
*   Використовуй метод `includes()` для перевірки, чи масив `friends` містить `friendName`.

  

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

  

const allUsers \= \[
  {
    name: "Moore Hensley",
    friends: \["Sharron Pace"\]
  },
  {
    name: "Sharlene Bush",
    friends: \["Briana Decker", "Sharron Pace"\]
  },
  {
    name: "Ross Vazquez",
    friends: \["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"\]
  },
  {
    name: "Elma Head",
    friends: \["Goldie Gentry", "Aisha Tran"\]
  },
  {
    name: "Carey Barr",
    friends: \["Jordan Sampson", "Eddie Strong"\]
  },
  {
    name: "Blackburn Dotson",
    friends: \["Jacklyn Lucas", "Linda Chapman"\]
  },
  {
    name: "Sheree Anthony",
    friends: \["Goldie Gentry", "Briana Decker"\]
  }
\];

console.log(getUsersWithFriend(allUsers, "Briana Decker")); 
// \[
//   {
//     name: "Sharlene Bush",
//     friends: \["Briana Decker", "Sharron Pace"\]
//   },
//   {
//     name: "Sheree Anthony",
//     friends: \["Goldie Gentry", "Briana Decker"\]
//   }
// \]

console.log(getUsersWithFriend(allUsers, "Goldie Gentry"));
// \[
//   {
//     name: "Elma Head",
//     friends: \["Goldie Gentry", "Aisha Tran"\]
//   },
//   {
//     name: "Sheree Anthony",
//     friends: \["Goldie Gentry", "Briana Decker"\]
//   }
// \]

console.log(getUsersWithFriend(allUsers, "Adrian Cross" )); // \[\]

Залиш цей код для перевірки ментором.

  

**На що буде звертати увагу ментор при перевірці:**

*   Оголошена змінна `getUsersWithFriend`
*   Змінній `getUsersWithFriend` присвоєна стрілочна функція з параметрами `(users, friendName)`
*   Для перебирання параметра `users` використовується метод `filter()`
*   Якщо значення параметра `friendName` — це рядок `"Briana Decker"`, функція повертає масив об'єктів користувачів з іменами `Sharlene Bush` і `Sheree Anthony`
*   Якщо значення параметра `friendName` — це рядок `"Goldie Gentry"`, функція повертає масив об'єктів користувачів з іменами `Elma Head` і `Sheree Anthony`
*   Якщо значення параметра `friendName` — це рядок `"Adrian Cross"`, функція повертає порожній масив
*   Виклик функції з випадковими, але валідними аргументами повертає правильне значення

  

  

**Задача 3.** **Сортування за кількістю друзів**

Виконуй це завдання у файлі `task-3.js`

  

Напиши стрілочну функцію `sortByDescendingFriendCount(users)` , яка прийматиме один параметр `users` — масив об’єктів користувачів.

Функція має повертати масив усіх користувачів, відсортованих за спаданням кількостій їх друзів (властивість `friends`).

  

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

  

console.log(
  sortByDescendingFriendCount(\[
    {
      name: "Moore Hensley",
      friends: \["Sharron Pace"\],
      gender: "male"
    },
    {
      name: "Sharlene Bush",
      friends: \["Briana Decker", "Sharron Pace"\],
      gender: "female"
    },
    {
      name: "Ross Vazquez",
      friends: \["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"\],
      gender: "male"
    },
    {
      name: "Elma Head",
      friends: \["Goldie Gentry", "Aisha Tran"\],
      gender: "female"
    },
    {
      name: "Carey Barr",
      friends: \["Jordan Sampson", "Eddie Strong"\],
      gender: "male"
    },
    {
      name: "Blackburn Dotson",
      friends: \["Jacklyn Lucas", "Linda Chapman"\],
      gender: "male"
    },
    {
      name: "Sheree Anthony",
      friends: \["Goldie Gentry", "Briana Decker"\],
      gender: "female"
    }
  \])
);
// \[
//   {
//     name: "Ross Vazquez",
//     friends: \["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"\],
//     gender: "male"
//   },
//   {
//     name: "Sharlene Bush",
//     friends: \["Briana Decker", "Sharron Pace"\],
//     gender: "female"
//   },
//   {
//     name: "Elma Head",
//     friends: \["Goldie Gentry", "Aisha Tran"\],
//     gender: "female"
//   },
//   {
//     name: "Carey Barr",
//     friends: \["Jordan Sampson", "Eddie Strong"\],
//     gender: "male"
//   },
//   {
//     name: "Blackburn Dotson",
//     friends: \["Jacklyn Lucas", "Linda Chapman"\],
//     gender: "male"
//   },
//   {
//     name: "Sheree Anthony",
//     friends: \["Goldie Gentry", "Briana Decker"\],
//     gender: "female"
//   },
//   {
//     name: "Moore Hensley",
//     friends: \["Sharron Pace"\],
//     gender: "male"
//   }
// \]

Залиш цей код для перевірки ментором.

  

**На що буде звертати увагу ментор при перевірці:**

*   Оголошена змінна `sortByDescendingFriendCount`
*   Змінній `sortByDescendingFriendCount` присвоєна стрілочна функція з параметром `(users)`
*   Для перебирання параметра `users` використаний метод `toSorted()`
*   Виклик функції із зазначеним масивом `users` повертає новий масив користувачів, відсортований за спаданням кількості їхніх друзів
*   Виклик функції з випадковими, але валідними аргументами повертає правильне значення

  

  

**Задача 4**. **Загальний баланс**

  

Напиши стрілочну функцію `getTotalBalanceByGender(users, gender)`, яка прийматиме два параметра:

*   перший параметр `users` — масив об’єктів користувачів,
*   другий параметр `gender` — рядок, що зберігає стать.

  

Функція має використовувати ланцюжок виклику методів та повертати загальний баланс користувачів (властивість `balance`), стать яких (властивість `gender`) збігається зі значенням параметра `gender`.

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

  

const clients \= \[
	{
    name: "Moore Hensley",
    gender: "male",
    balance: 2811
  },
  {
    name: "Sharlene Bush",
    gender: "female",
    balance: 3821
  },
  {
    name: "Ross Vazquez",
    gender: "male",
    balance: 3793
  },
  {
    name: "Elma Head",
    gender: "female",
    balance: 2278
  },
  {
    name: "Carey Barr",
    gender: "male",
    balance: 3951
  },
  {
    name: "Blackburn Dotson",
    gender: "male",
    balance: 1498
  },
  {
    name: "Sheree Anthony",
    gender: "female",
    balance: 2764
  }
\];

console.log(getTotalBalanceByGender(clients, "male")); // 12053

console.log(getTotalBalanceByGender(clients, "female")); // 8863

Залиш цей код для перевірки ментором.

  

**На що буде звертати увагу ментор при перевірці:**

*   Оголошена змінна `getTotalBalanceByGender`
*   Змінній `getTotalBalanceByGender` присвоєна стрілочна функція з параметрами `(users, gender)`
*   У тілі функції використовується ланцюжок методів у правильному порядку
*   Значення параметра `users` не змінюється
*   Якщо значення параметра `gender` — це рядок `"male"`, функція повертає число `12053`
*   Якщо значення параметра `gender` — це рядок `"female"`, функція повертає число `8863`
*   Виклик функції з випадковими, але валідними аргументами повертає правильне значення
