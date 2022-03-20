```python
#(1)求三角形的底,高,面积
b = int(input('输入三角形底数: '));
h = float(input('输入三角形高: '));
area = b*h*0.5;
print('三角形面积为 %f' %area);
```


```python
#(2)求三角形的周长
a = float(input('输入三角形第一边长: '));
b = float(input('输入三角形第二边长: '));
c = float(input('输入三角形第三边长: '));
s = (a + b + c) ;
print('三角形周长为 %0.2f' %s);
```


```python
#(3)求矩形的周长,面积
a = float(input('输入矩形长: '));
b = float(input('输入矩形宽: '));
s = (a+b)*2;
area=a*b;
print('矩形的周长为 %f' %s);
print('矩形的面积为 %f' %area);
```

    输入矩形长: 12
    输入矩形宽: 3
    矩形的周长为 30.000000
    矩形的面积为 36.000000
    


```python
#(4)求圆的面积和周长
radius = float(input('输入圆形的半径:'));
len=2*3.14*radius;
print("圆形周长:",len);
area=3.14*radius*radius;
print("圆形面积:",area);
```

    输入圆形的半径:12
    圆形周长: 75.36
    圆形面积: 452.15999999999997
    


```python
#(5)计算y=2x-2斜率,xy截距
def getSlope(x1,y1,x2,y2):
    return (y2-y1)/(x2-x1);

#计算x截距
def getXIntercept():
    return 1;

#计算y截距
def getYIntercept():
    return -2;

print("截距:",getSlope(2,2,6,10));
print("x截距:",getXIntercept());
print("y截距:",getYIntercept());
```

    截距: 2.0
    x截距: 1
    y截距: -2
    


```python
# 求两点之间的距离
import math;
p1=[2,2];
p2=[6,10];
xielv=abs((p1[1]-p2[1])/(p1[0]-p2[0]));
juli= math.sqrt((p1[1]-p2[1])*(p1[1]-p2[1])+(p1[0]-p2[0])*(p1[0]-p2[0]));
print(xielv);
print (juli);
```


```python
#(6) y=x^2+6x+9  求x使y=0
def getY(x):
    return x*x+6*x+9;

for x in range(-5,5):
    if getY(x)== 0:
        print("x=",x,"y=",getY(x));
        break;
```

    x= -3 y= 0
    0
    


```python
#(7)求"python" 和 "datascience" 的长度
print(len("python"));
print(len("datascience"))
```

    6
    11
    


```python
#(13) and检查python和cannon是否都存在on
import re;
print(re.search("on","python")!=None and re.search("on","connon")!=None);
```

    True
    


```python
#(14) in的用法, 一句话是否包含行话
if "ss" in "asdasdasssssasd":
    print("yes");
else:
    prinn("no");
```

    yes
    


```python
#(15)python和connon中都没有 on
import re;
print(re.search("on","python")==None and re.search("on","connon")==None);
```

    False
    


```python
#(16) 找到python文本的长度
print(str(float(len("python"))));
```

    6.0
    


```python
#(17) 奇书偶数
num=int(input('enter number'));
if(num%2==0):
 print ('number is even');
else:
 print ('number is odd');
```


```python
#(18) 
print(7/3);
print((7/3)==2.7)
```

    2.3333333333333335
    False
    


```python
#(19)检查"10"和10的类型
print(type("10")==type(10));
```

    False
    


```python
#(20)检查int("9.6")是否等于10
print(int(float("9.6"))==10);
```

    False
    


```python
#(21)0作为被除数
def divide(a,b):
    if(b == 0):
        return "null";
    return str(a/b);
print(divide(1,0));
```


```python
import re
line="this hdr-biz model server"
pattern=r"hdr-biz"
m = re.search(pattern, line)
print(m)
```

    <_sre.SRE_Match object; span=(5, 12), match='hdr-biz'>
    


```python
print(str(12.121));
print(repr(12.12312))
print(int("123"))
```

    12.121
    12.12312
    123
    


```python
print(type("asdas"))
print(type(123))
```

    <class 'str'>
    <class 'int'>
    


```python
def equals(a,b):
    int(a);
    int(b);
    return a==b;
print(equals("10",10));
```

    False
    
