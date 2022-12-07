# Solutions

### Day 1
First part: 
```python
max([sum(map(int, elf.split('\n'))) for elf in elves.split('\n\n')])
```

Second part: 
```python
sum(sorted([sum(map(int, elf.split('\n'))) for elf in elves.split('\n\n')])[-3:])
```

### Day 2
First part: 
```python
sum([{'A X':4,'A Y':8,'A Z':3,'B X': 1,'B Y':5,'B Z':9,'C X':7,'C Y':2,'C Z':6}[row] for row in text.split('\n')])
```

Second part: 
```python
sum([{'A X':3,'A Y':4,'A Z':8,'B X':1,'B Y':5,'B Z':9,'C X': 2,'C Y':6,'C Z':7}[row] for row in text.split('\n')])
```

### Day 3
First part: 
```python
sum([ord(item) - 38 if item.isupper() else ord(item) - 96  for item in [list(set(line[:len(line)//2]) & set(line[len(line)//2:]))[0] for line in text.split('\n')]])
```

Second part: 
```python
# I did not find a one line solution  (aka. was too lazy to find it)
```

### Day 3
First part: 
```python
sum([1 for (a,b),(c,d) in [(list(map(int, a.split('-'))), list(map(int, b.split('-')))) for a,b in [abc.split(',') for abc in text.split('\n')]] if (set(range(a,b+1)).issubset(set(range(c,d+1)))) or (set(range(c,d+1)).issubset(set(range(a,b+1))))])
```

Second part: 
```python
sum([1 for (a,b),(c,d) in [(list(map(int, a.split('-'))), list(map(int, b.split('-')))) for a,b in [abc.split(',') for abc in text.split('\n')]] if (len(set(range(a,b+1)) & set(range(c,d+1)))) > 0])
```

### Day 4
First part & second part:
```python
# I solved it using class MyStack and for loop.
```

### Day 5
First part: 
```python
min([i+3 for i in range(len(text) - 3) if len(text[i:i+3]) == len(set(text[i:i+3]))])
```

Second part: 
```python
min([i+14 for i in range(len(text) - 14) if len(text[i:i+14]) == len(set(text[i:i+14]))])
```

### Day 6
First part & second part:
```python
# Definitelly not doing this using oneliner :D My code had about 100 lines.
```
