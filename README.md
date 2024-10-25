# 1 

x1 = int(input("Введите время в секундах прошедшее с начала дня\n"))
if x > 86400:
    print("Столько секунд нету в сутках")
else:
    choice = int(input("Посчитать сколько осталось времени до полуночи в\n1 - часах\n2 - минутах\n3 - секундах\n"))
    if choice == 1:
        print(f"До полуночи осталось {round(((86400 - x) / 60) / 60,2)} часов")
    elif choice == 2:
        print(f"До полуночи осталось {round((86400 - x) / 60, 2)} минут")
    elif choice == 3:
        print(f"До полуночи осталось {86400 - x} секунд")

# 2 
x = int(input("Введите диаметр окружности: "))
choice = int(input("1 - Площадь\n2 - Периметр\n"))
p = 3.14159265
r = x / 2
if choice == 1:
    print(f"Площадь = {round( 2 * p * r , 2)}")
elif choice == 2:
    print(f"Периметр = {round(p * (r**2) , 2)}")

# 3 

q = int(input("Введите стоимость приставки: "))
w = int(input("Введите кол-во приставок: "))
e = int(input("Введите процент скидки: "))
choice = int(input("1 - общая сумма заказа\n2 - стоимость одной приставки со скидкой\n"))
if choice == 1:
    print(f"Общая стоимость заказа = {(q - (q * w / 100)) * e}")
elif choice == 2:
    print(f"Стоимость одной приставки = {q - (q * w / 100)}")

# 5 
hour = int(input("Введите количество часов: "))

if hour > 24:
    print("Столько часов в сутках нету(")
else:
    if hour >= 0 and hour < 6:
        print("Good Night")
    elif hour >= 6 and hour < 13:
        print("Good Morning")
    elif hour >= 13 and hour < 17:
        print("Good Day")
    elif hour >= 17 and hour < 0:
        print("Good Evening")
