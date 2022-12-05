# AoC 2022

The PROHIBITED way of solving a puzzle

Objective: Solve with the shortest js code possible

Day 1:
- Ugh!
- Go to [https://adventofcode.com/2022/day/1/input](https://adventofcode.com/2022/day/1/input)
- Part 1 run ```eval(`Math.max(${document.body.textContent.replace(/\n\n/g,',').replace(/\n/g,'+')}0)`)```
- Part 2 run ```eval(eval(`[${document.body.textContent.replace(/\n\n/g,',').replace(/\n/g,'+')}0]`).sort((a,b)=>b-a).slice(0,3).join('+'))```

Day 2 (interesting the way that rock,paper,scissors was logically simplified, without ifs):
- Terrible!
- Go to [https://adventofcode.com/2022/day/2/input](https://adventofcode.com/2022/day/2/input)
- Part 1 run ```eval(document.body.textContent.split('\n').map(x=>x?(a='XYZ'.indexOf(x[2]),a+1+(a+4-'ABC'.indexOf(x[0]))%3*3):0).join('+'))```
- Part 2 run ```eval(document.body.textContent.split('\n').map(x=>x?(a='XYZ'.indexOf(x[2]),a*3+1+(a+'ABC'.indexOf(x[0])+2)%3):0).join('+'))```

Day 3:
- AaAa!
- Go to [https://adventofcode.com/2022/day/3/input](https://adventofcode.com/2022/day/3/input)
- Part 1 run ```document.body.textContent.trim().split('\n').map(m=>(d=m.length,l=[...m.slice(0,d/2)].find(c=>[...m.slice(d/2)].some(_c=>c==_c)),f='charCodeAt',l==l.toUpperCase()?l[f](0)-38:(l[f](0)-96))).reduce((a,b)=>a+b)```
- Part 2 run ```[...document.body.textContent.matchAll(/(.*)\n(.*)\n(.*)\n/g)].map(z=>(f='charCodeAt',l=[...z[1]].find(c=>[...z[2]].some(v=>[...z[3]].some(b=>c==v&v==b))),l==l.toUpperCase()?l[f](0)-38:(l[f](0)-96))).reduce((a,b)=>a+b)```

Day 4:
- UaUaUa!
- Go to [https://adventofcode.com/2022/day/4/input](https://adventofcode.com/2022/day/4/input)
- Part 1 run ```document.body.textContent.trim().split('\n').map(l=>l.split(/\D/).map(Number)).reduce((a,[h,j,k,l])=>a+((h<=k&k<=l&l<=j)|(k<=h&h<=j&j<=l)),0)```
