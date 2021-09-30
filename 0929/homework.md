# 輸入與輸出
```
python: 輸入input() 
使用輸入函數得到的資料型態會是str(字串)
python: 輸出ootput()
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
```
int()函數與eval()函數
把字串轉換成數字

```
```
score = int(input("please enter your score:")) #把str 改成int

print(score+10)
```
![image](https://user-images.githubusercontent.com/90738394/135380576-03fd474c-f18c-475b-8b6b-319edff5060f.png)
