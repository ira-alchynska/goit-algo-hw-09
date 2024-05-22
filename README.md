# Comparison of Coin Change Algorithms Efficiency

## Problem Description

It is necessary to develop two functions for a cash register system that provides change to a customer:

1. A greedy algorithm function `find_coins_greedy`.
2. A dynamic programming function `find_min_coins`.

## Greedy Algorithm

### Working Principle

The greedy algorithm works by choosing the highest available coin denomination until the amount is reduced to zero. This approach does not always guarantee the minimum number of coins but is very fast to execute.

### Complexity

The time complexity of the greedy algorithm is O(n), where n is the number of different coin denominations. In our case, this is always 6, so the complexity is effectively constant O(1).

## Dynamic Programming Algorithm

### Working Principle

The dynamic programming algorithm uses a table to store the minimum number of coins needed for each possible amount from 0 to the given amount. It guarantees the minimum number of coins for any amount.

### Complexity

The time complexity of the dynamic programming algorithm is O(m * n), where m is the amount, and n is the number of different coin denominations.

## Efficiency Comparison

### Performance for the Amount 113

- Greedy Algorithm:
  - Result: {50: 2, 10: 1, 2: 1, 1: 1}
  - Execution Time: Very fast, almost instantaneous.

- Dynamic Programming:
  - Result: {1: 1, 2: 1, 10: 1, 50: 2}
  - Execution Time: Slightly longer, but still fast for small amounts.

### Large Amounts

For large amounts, dynamic programming may be slower due to the need to process many subproblems. However, it guarantees the minimum number of coins. The greedy algorithm remains fast but may not find the optimal solution.

## Conclusions

The greedy algorithm is suitable for quickly obtaining a result in most practical cases where the set of denominations always allows finding an optimal solution. The dynamic programming algorithm is more general and versatile but requires more time for large amounts.



# Порівняння ефективності алгоритмів розбиття суми на монети

## Опис задачі

Необхідно розробити дві функції для касової системи, яка видає решту покупцеві:

1. Функція жадібного алгоритму `find_coins_greedy`.
2. Функція динамічного програмування `find_min_coins`.

## Жадібний алгоритм

### Принцип роботи

Жадібний алгоритм працює за принципом вибору найбільшого доступного номіналу монет, поки сума не буде зменшена до нуля. Цей підхід не завжди гарантує мінімальну кількість монет, але є дуже швидким у виконанні.

### Складність

Часова складність жадібного алгоритму - O(n), де n - кількість різних номіналів монет. У нашому випадку, це завжди 6, тому складність фактично постійна O(1).

## Алгоритм динамічного програмування

### Принцип роботи

Алгоритм динамічного програмування використовує таблицю для збереження мінімальної кількості монет, необхідних для кожної можливої суми від 0 до заданої суми. Він гарантує мінімальну кількість монет для будь-якої суми.

### Складність

Часова складність алгоритму динамічного програмування - O(m * n), де m - сума, а n - кількість різних номіналів монет.

## Порівняння ефективності

### Виконання на сумі 113

- Жадібний алгоритм:
  - Результат: {50: 2, 10: 1, 2: 1, 1: 1}
  - Час виконання: дуже швидкий, майже миттєвий.

- Динамічне програмування:
  - Результат: {1: 1, 2: 1, 10: 1, 50: 2}
  - Час виконання: трохи довше, але все ще швидкий для малих сум.

### Великі суми

Для великих сум динамічне програмування може бути повільнішим через необхідність обробки великої кількості підсум. Однак, воно гарантує мінімальну кількість монет. Жадібний алгоритм залишається швидким, але може не знайти оптимального рішення.

## Висновки

Жадібний алгоритм підходить для швидкого отримання результату в більшості практичних випадків, де набір номіналів дозволяє завжди знайти оптимальне рішення. Алгоритм динамічного програмування є більш загальним та універсальним, але потребує більше часу для великих сум.


