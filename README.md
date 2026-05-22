# laba-3.1
# Задание task_03_01_14.
#
# Выполнил: Котова Е.А.
# Группа: ЦИБ-251

def split_numbers(*args):
    - list: отрицательные значения (отсортированы по убыванию);
    - list: неотрицательные значения (отсортированы по возрастанию).
    
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
