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

 1:'
＋＋＋
＋・＋
＋＋＋'
,2:'
＋＋＋　　　
・・・
＋＋＋'
,3:'
＋・＋
＋・＋
＋・＋'
,4:'
・・・
・・・
・・・'
,5:'
壁・壁
・・・
壁・壁'
```
```
mapfill(cx,cy,deco)
```
```
(Array(40*40+1).join('壁')).match(/.{1,40}/g)
```
