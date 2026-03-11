# Задание 2 из ЕГЭ по информатике
## №15970 https://inf-ege.sdamgia.ru/problem?id=15970
### <img width="854" height="265" alt="image" src="https://github.com/user-attachments/assets/5e1784d2-40ff-4643-9ec5-1e6bec3fb292" />
### Используем для этого скрипт:
```
print ('x y w z')
for x in range(2):
    for y in range(2):
        for w in range(2):
            for z in range(2):
                if not ((x and (not y)) or (y == z) or w):
                    print(x, y, w, z)
```
### Все выданные варианты:
### x y w z
### 0 0 0 1
### 0 1 0 0
### 1 1 0 0
### Cопоставив цифры, видно что ответ: *yxwz*

## №16377 https://inf-ege.sdamgia.ru/problem?id=16377
## <img width="843" height="257" alt="image" src="https://github.com/user-attachments/assets/cb6d09dc-d8d9-41f3-be70-1e7559d9a3fd" />
### Используем скрипт:
```
print ('x y w z')
for x in range(2):
    for y in range(2):
        for w in range(2):
            for z in range(2):
                if (((x <= y) == (y <= z)) and (y or w)):
                    print (x, y, w, z)
```
### Все выданные варианты:
### x y w z
### 0 0 1 0
### 0 0 1 1
### 0 1 0 1
### 0 1 1 1
### 1 1 0 1
### 1 1 1 1
### Cопоставив цифры, видно что ответ: *xzwy*

## №16431 [https://inf-ege.sdamgia.ru/problem?id=15970](https://inf-ege.sdamgia.ru/problem?id=16431)
### <img width="846" height="265" alt="image" src="https://github.com/user-attachments/assets/d1935bd0-ed3b-491d-a9ce-990a90b1b771" />
### Используем скрипт:
```
print ('x y w z')
for x in range(2):
    for y in range(2):
        for w in range(2):
            for z in range(2):
                if (((y <= x) == (x <= w)) and (z or x)):
                    print (x, y, w, z)
```
### Все выданные варианты:
### x y w z
### 0 0 0 1
### 0 0 1 1
### 1 0 1 0
### 1 0 1 1
### 1 1 1 0
### 1 1 1 1
### Cопоставив цифры, видно что ответ: *ywxz*


# Задание 8 из ЕГЭ по информатике
## №17328 https://inf-ege.sdamgia.ru/problem?id=17328
## <img width="860" height="35" alt="image" src="https://github.com/user-attachments/assets/21efd610-6a7d-444d-a2a9-1a7bfac0e185" />
```
b = 'ЕАИ'
a = 'ГРСМ'
c = 0
for i in a:
    for j in b:
        for n in a:
            for m in b:
                for l in a:
                    for k in b:
                        for g in a:
                            s =i+j+n+m+l+k+g
                            f = set(s)
                            if len(f) == len(s):
                                c += 1
print(c)
```
### Ответ: 144

## №18079 [https://inf-ege.sdamgia.ru/problem?id=17328](https://inf-ege.sdamgia.ru/problem?id=18079)
## <img width="841" height="49" alt="image" src="https://github.com/user-attachments/assets/ffbc331f-cbf4-4ee0-9baa-b6be5b974ca0" />

```
count = 0
letters = ['К', 'О', 'Т']

# Перебираем все возможные комбинации из 6 букв
for a in letters:
    for b in letters:
        for c in letters:
            for d in letters:
                for e in letters:
                    for f in letters:
                        word = a + b + c + d + e + f
                        # Считаем, сколько раз встречается буква К
                        if word.count('К') == 1:
                            count += 1

print(count)
```
### Ответ: 192

## №18491 [inf-ege.sdamgia.ru/problem?id=18491](https://inf-ege.sdamgia.ru/problem?id=18491)
## <img width="837" height="33" alt="image" src="https://github.com/user-attachments/assets/cfcd6d92-391f-4825-946a-fa3c01ec3657" />

```
a1=['о','л','г','а']
a=['о','л','г','а','ь']
k=0
for b1 in a1:
    for b2 in a:
        for b3 in a:
            for b4 in a:
                for b5 in a:
                    s=b1+b2+b3+b4+b5
                    if s.count('о')==1 and s.count('л')==1 and s.count('ь')==1 and s.count('г')==1 and s.count('а')==1 :
                        if not('оь') in s and not('аь') in s:
                            k+=1
print(k)
```
### Ответ: 48
