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
#did not find a one line solution 
```
