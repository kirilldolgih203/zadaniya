def find_division_index(arr):
    if arr != sorted(arr):
        arr.sort()
    
    left, right = 0, len(arr) - 1
    
    while left <= right:
        mid = (left + right) // 2
        
        if arr[mid] == 1 and (mid == 0 or arr[mid-1] == 0):
            return mid
        elif arr[mid] == 0:
            left = mid + 1
        else:
            right = mid - 1
    
    return -1

arr = list(map(int, input("Введите упорядоченный массив из 0 и 1 через пробел: ").split()))

result = find_division_index(arr)
if result == -1:
    print("Разделение не найдено")
else:
    print("Место разделения: Индекс", result)
