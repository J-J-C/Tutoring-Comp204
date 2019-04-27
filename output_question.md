```python
word = "xyz123!@#"
  for i in range(len(word)-1, -2, -1):
    print (i, word[i], end='')
    if word[i].isdigit():
      for j in range(int(word[i])):
        print ("*", end='')
    print()
```
---
```python
def foo(a):
  if a.isdigit():
    print (a)

data1 = "5,10,15"
for item in data1:
  foo(item)

print ("----")

data2 = data1.split(",")

for item in data2:
  foo(item)
```
---
```python
code = { 6:["t", "g"], 14:["p","q"], 15:["c", "d"], 9:["o", "a"] }
data = "5,0:3,1:2,0"
splitdata = data.split(":")
for item in splitdata:
  splititem = item.split(",")
  print ( code[ int(splititem[0])*3 ][ int(splititem[1]) ], end="")
```

```python

```

```python

```
