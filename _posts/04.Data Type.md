# Data Type


```python
# List 
a_list = [1,2,3,4,5]

print(a_list)
print(a_list[0])
print(a_list[1])
```

    [1, 2, 3, 4, 5]
    1
    2
    


```python
# 슬라이싱 
print(a_list[:2])
```

    [1, 2]
    


```python
print(a_list[2:])
```

    [3, 4, 5]
    


```python
print(a_list[:])
```

    [1, 2, 3, 4, 5]
    


```python
print(a_list[1::2])
```

    [2, 4]
    


```python
b = a_list[:] #깊은 복사 <-> 얕은 복사는 주소만 복사되는 것. 
b[0] = 100
print(b)
```

    [100, 2, 3, 4, 5]
    


```python
print(a_list)
```

    [10, 2, 3, 4, 5]
    


```python
b_list = [] 
b_list.append(1) 
b_list.append(2) 
b_list.append(3) 

print(b_list)
```

    [1, 2, 3]
    


```python
b_list.insert(2,100) # 인덱스 2자리에 100을 추가한다.
print(b_list)
```

    [1, 2, 100, 3]
    


```python
# tuple 
a_tuple = (1,2,3,4,5)

print(a_tuple)
```

    (1, 2, 3, 4, 5)
    


```python
a_tuple[0] = 10 # 오류. 튜플은 한 번 정의하고 나면 인덱스로 값을 넣을 수 없음. 
# print(a_tuple)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Input In [19], in <cell line: 1>()
    ----> 1 a_tuple[0] = 10 
          2 print(a_tuple)
    

    TypeError: 'tuple' object does not support item assignment



```python
a = 100
b = 200 
a, b = b, a 
print(a)
```

    200
    


```python
# Dict 
a_dic = {1:'a', 'b':[1,2,3], 'c':3}
print(a_dic)
```

    {1: 'a', 'b': [1, 2, 3], 'c': 3}
    


```python
print(a_dic[1])
print(a_dic['b'])
print(a_dic['c'])
```

    a
    [1, 2, 3]
    3
    


```python
a_dic['d'] = 'Microsoft AI School'
print(a_dic)
```

    {1: 'a', 'b': [1, 2, 3], 'c': 3, 'd': 'Microsoft AI School'}
    


```python
# Set
a_set = {1,2,3}

print(a_set)
print(type(a_set))
```

    {1, 2, 3}
    <class 'set'>
    


```python
b_set = {3,4,5}
```


```python
a_set.union(b_set) #합집합
```




    {1, 2, 3, 4, 5}




```python
a_set.intersection(b_set) #교집합
```




    {3}




```python
a_set - b_set #차집합 
```




    {1, 2}




```python
a_set | b_set 
```




    {1, 2, 3, 4, 5}




```python
a_set & b_set 
```




    {3}




```python
# 부록

a = set((1,2,3)) # type변경  
print(a)
```

    {1, 2, 3}
    


```python
b = list(a) 
print(b)
```

    [1, 2, 3]
    


```python
c = tuple(b)
print(c)
print(type(c))
```

    (1, 2, 3)
    <class 'tuple'>
    


```python

```
