import random

options = ["Камінь", "Ножиці", "Папір"]

computer = random.choice(options)

user = input("Введи свій варіант (Камінь, Ножиці або Папір): ")

if user == computer:
    print("Нічия!")
elif user == "Камінь" and computer == "Ножиці":
    print("Ти переміг! Камінь ламає ножиці.")
elif user == "Камінь" and computer == "Папір":
    print("Ти програв! Папір обгортає камінь.")
elif user == "Ножиці" and computer == "Папір":
    print("Ти переміг! Ножиці ріжуть папір.")
elif user == "Ножиці" and computer == "Камінь":
    print("Ти програв! Камінь ламає ножиці.")
elif user == "Папір" and computer == "Камінь":
    print("Ти переміг! Папір обгортає камінь.")
elif user == "Папір" and computer == "Ножиці":
    print("Ти програв! Ножиці ріжуть папір.")
else:
    print("Невірний ввід. Спробуй ще раз.")
