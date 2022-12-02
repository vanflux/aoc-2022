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
- Part 1 run ```eval(document.body.textContent.trim().split('\n').map(x=>(b='charCodeAt',a=x[2][b](0)-88,a+1+(a+(4-(x[0][b](0)-65)))%3*3)).join('+'))```
- Part 2 run ```eval(document.body.textContent.trim().split('\n').map(x=>(b='charCodeAt',a=x[2][b](0)-88,a*3+1+(a+x[0][b](0)-63)%3)).join('+'))```
