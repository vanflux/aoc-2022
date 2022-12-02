# AoC 2022

The PROHIBITED way of solving a puzzle

Objective: Solve with the shortest js code possible

Day 1:
- Ugh!
- Go to [https://adventofcode.com/2022/day/1/input](https://adventofcode.com/2022/day/1/input)
- Run ```eval(`Math.max(${document.body.textContent.replace(/\n\n/g,',').replace(/\n/g,'+')}0)`)``` on the console

Day 2:
- Terrible!
- Go to [https://adventofcode.com/2022/day/2/input](https://adventofcode.com/2022/day/2/input)
- Run ```eval(document.body.textContent.trim().split('\n').map(x=>(b='charCodeAt',a=x[2][b](0)-88,a+1+(a+(4-(x[0][b](0)-65)))%3*3)).join('+'))``` on the console
