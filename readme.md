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
