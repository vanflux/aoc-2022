# AoC 2022

The PROHIBITED way of solving a puzzle

Objective: Solve with the shortest js code possible

Day 1:
- Ugh!
- Go to [https://adventofcode.com/2022/day/1/input](https://adventofcode.com/2022/day/1/input)
- Part 1 run ```eval(`Math.max(${document.body.textContent.replace(/\n\n/g,',').replace(/\n/g,'+')}0)`)```
- Part 2 run ```eval(eval(`[${document.body.textContent.replace(/\n\n/g,',').replace(/\n/g,'+')}0]`).sort((a,b)=>b-a).slice(0,3).join('+'))```

Day 2:
- Terrible!
- Go to [https://adventofcode.com/2022/day/2/input](https://adventofcode.com/2022/day/2/input)
- Part 1 run ```eval(document.body.textContent.split('\n').map(x=>x?(a='XYZ'.indexOf(x[2]),a+1+(a+4-'ABC'.indexOf(x[0]))%3*3):0).join('+'))```
- Part 2 run ```eval(document.body.textContent.split('\n').map(x=>x?(a='XYZ'.indexOf(x[2]),a*3+1+(a+'ABC'.indexOf(x[0])+2)%3):0).join('+'))```
