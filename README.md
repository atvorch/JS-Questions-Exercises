# JS-Questions-Exercises
JS Questions &amp; Exercises


## Задания
1.Реализуйте функцию isPrime(), которая возвращает true или false, указывая, является ли переданное ей число простым.
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
