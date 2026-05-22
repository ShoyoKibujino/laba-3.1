# laba-3.1
# Задание task_03_01_14.
# Условие: Напишите функцию, которая принимает неограниченное количество числовых
аргументов и возвращает кортеж из двух списков:
- отрицательных значений (отсортирован по убыванию);
- неотрицательных значений (отсортирован по возрастанию).
# Выполнил: Котова Е.А.
# Группа: ЦИБ-251

def split_numbers(*args):
    
    otric = []
    neotric = []
    
    for x in args:
        if x < 0:
            otric.append(x)
        else:
            neotric.append(x)
            
    otric.sort(reverse=True)
    neotric.sort()
    return (otric, neotric)

print(split_numbers(1, 4, -5, 0, -33))
