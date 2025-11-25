# Fibonacci_detector_byJamshid

def fibonacci():

    print("Добро пожаловать на программу детектор Фибоначчи!")

    while True:
        # --- Выбор режима ---
        try:
            choice = int(input(
                "Выберите функцию:\n"
                "1 - Показать все числа Фибоначчи до указанного числа.\n"
                "2 - Проверить, является ли число Фибоначчи.\n"
            ))
        except ValueError:
            print("Введите только цифру 1 или 2.")
            continue

        # --- Функция №1 ---
        if choice == 1:
            def fibonachi_calc():
                n = int(input("Введите число: "))
                a = 0
                b = 1
                while a <= n:
                    print(a)
                    c = a + b
                    a = b
                    b = c
            fibonachi_calc()

        # --- Функция №2 ---
        elif choice == 2:
            def fibonachi_num():
                n = int(input("Введите число: "))
                a = 0
                b = 1
                while a < n:
                    c = a + b
                    a = b
                    b = c
                if a == n:
                    print("Ваше число является числом Фибоначчи.")
                else:
                    print("Ваше число НЕ является числом Фибоначчи.")
            fibonachi_num()

        else:
            print("Выберите правильный вариант!")
            continuej

        # --- Повторить? ---
        try:
            final_q = int(input("Хотите продолжить?\n1 - Да\n2 - Нет\n"))
        except ValueError:
            print("Введите только 1 или 2.")
            continue

        if final_q == 1:
            continue
        else:
            print("До свидания! Желаем вам удачи :)")
            break


fibonacci()
