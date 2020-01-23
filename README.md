# bomb
random dungeon maker

```
1. size 40*40
2. decide the bom number 2-20
3. bom decolation
4. bom to bom is road
5. set stair bom center 
```
```
bom decolation

t1
＋
t2
・＋・
t3
・
＋
・
t4
・・・
・＋・
・・・
t5
　・
・＋・
　・
t6
　　・
・＋・
　　・
t7
　・
　＋
・・・
t8
・
・＋・
・
t9
　　・
・＋・
　　・
```
```
(Array(40*40+1).join('壁')).match(/.{1,40}/g)
```
