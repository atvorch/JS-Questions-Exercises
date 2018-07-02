# JS-Questions-Exercises
JS Questions &amp; Exercises


## Задания
1. Реализуйте функцию isPrime(), которая возвращает true или false, указывая, является ли переданное ей число простым.
```javascript
const isPrime = (number) => {
    if (number < 2) {
        return false;
    }

    for (let i = 2; i < number; i += 1) {
        if (number % i === 0) {
        return false;
        }
    }

    return true;
};
```
1. Реализуйте функцию factorial(), которая возвращает факториал переданного ей числа.
```javascript
const factorial = num => {
    if (num <= 1) {
        return 1;
    }

    const iter = (count, acc) => {
        if (count === 1) {
            return acc;
        }

        return iter(count - 1, count * acc);
    };

    return iter(num, 1);
};
```
1. Реализуйте функцию fib(), возвращающую n-ное число Фибоначчи.
```javascript
const fib = n => n <= 1 ? n : fib(n - 1) + fib(n - 2);
};
```
