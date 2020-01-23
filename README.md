# bomb
random dungeon maker
https://codepen.io/gnjo/pen/gObqWae
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
let mapfill=(bm,x,y,deco)=>{
deco.split('\n').map((d,i)=>{
 d.split('').map((d,j)=>{
  let f=!((y+i>40)||(x+j>40)) && d!='＋'
  if(f)bm[y+i][x+j]=d
 }
})
 return bm;
}
```
```
(Array(40*40+1).join('壁')).match(/.{1,40}/g)

fn.randi=(min, max)=>{//int and include the max
  let a =Math.ceil(min) ,b= Math.floor(max||0);
  min=Math.min(a,b),max=Math.max(a,b)
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
```
