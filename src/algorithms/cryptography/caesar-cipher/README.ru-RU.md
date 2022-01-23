# Алгоритм шифра Цезаря

В криптографии **шифр Цезаря**, также известный как **шифр сдвига**, **код Цезаря** или **сдвиг Цезаря**, является одним из самых простых и широко известных методов шифрования. Это вид шифра подстановки, в котором каждый символ в открытом тексте заменяется символом, находящимся на некотором постоянном числе позиций левее или правее него в алфавите. Например, в шифре со сдвигом вправо на `3`, `D` была бы заменена на `A`, `E` станет `B`, и так далее. Метод назван в честь Юлия Цезаря, который использовал его в своей личной переписке.

![Алгоритм шифра Цезаря](https://upload.wikimedia.org/wikipedia/commons/4/4a/Caesar_cipher_left_shift_of_3.svg)

## Пример
Это преобразование можно представить как выравнивание двух алфавитов; алфавит шифра - это обычный алфавит, повёрнутый влево или вправо на некоторое количество позиций. Например, здесь приведен шифр Цезаря, использующий поворот влево на три позиции, что эквивалентно сдвигу вправо на 23 (параметр сдвига используется в качестве ключа):

```text
Обычный:    ABCDEFGHIJKLMNOPQRSTUVWXYZ
Шифрованный:   XYZABCDEFGHIJKLMNOPQRSTUVW
```

При шифровании человек просматривает каждую букву сообщения в "открытой" строке и записывает соответствующую букву в "шифрованной" строке.

```text
Обычный текст:     THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG
Шифрованный текст: QEB NRFZH YOLTK CLU GRJMP LSBO QEB IXWV ALD
```

## Сложность

- Время: `O(|n|)`
- Пространство: `O(|n|)`

## Ссылки

- [Шифр Цезаря на Wikipedia](https://ru.wikipedia.org/wiki/Шифр_Цезаря)