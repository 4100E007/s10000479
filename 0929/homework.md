# 輸入與輸出
```
python: 輸入input() 
使用輸入函數得到的資料型態會是str(字串)
python: 輸出output()
```
---
### example
```
a = input("please enter your name:")
print("welcome",a)

type(a) #查看a的資料型態

```
![git](https://user-images.githubusercontent.com/90738394/135252112-51cb060c-38fb-4cbe-91bd-484e164fb458.PNG)
```
老師希望能夠把分數加十分
score = input("please enter your score:")
print(score+10)
得到的結果卻是:
TypeError                                 Traceback (most recent call last)
<ipython-input-1-a91813643229> in <module>()
      1 score = input("please enter your score:")
----> 2 print(score+10)

TypeError: can only concatenate str (not "int") to str


```
```
TypeError:資料型態錯誤

```
# 更正過後的程式碼

```
int()函數與eval()函數
把字串轉換成數字

```
```
score = int(input("please enter your score:")) #把str 改成int

print(score+10)
```
![image](https://user-images.githubusercontent.com/90738394/135380576-03fd474c-f18c-475b-8b6b-319edff5060f.png)
# 格式化輸出
```
1.使用String modulo operator(%)
2.使用format 方法

```
# example 
```
使用format方式
print("i love {} from {} ".format("music","japan"))
```
![image](https://user-images.githubusercontent.com/90738394/135554116-6c1ef8c4-06db-4dd5-9c48-e7f880b4c665.png)
```
#使用指定位置表達
print("i love {1} from {0} ".format("music","japan"))
```
![image](https://user-images.githubusercontent.com/90738394/135554475-9af5acca-d8f8-46c9-8caa-9561d51a344c.png)
使用String modulo operator(%)
# 列印整數(integer)與 浮點數(float) 的值
print("Happy : %2d, Python : %5.2f" % (1, 05.333))
 
# 列印字串
print("Happy %s day" % ("python"))

![image](https://user-images.githubusercontent.com/90738394/135558492-69a76a39-43aa-45ca-99e5-23408709ad3e.png)
