# -
试一试
import random
number1 = random.randint(1,100)
min1 = 1
max1 = 100
i = 1
while 1:
    number = eval(input("Please enter a number between "+ str(min1) + " and "+ str(max1) + ":"))
    if number > int(number) or number < 0:
        print("请输入正整数！")
        continue
    if number == 0:
        print("退出游戏，下次再见！")
        break
    if number == number1:
        print("猜中了！")
    elif number > number1:
        max1 = int(number) - 1
        print("猜大了！")
    elif number < number1:
        min1 = int(number) + 1
        print("猜小了！")
    if i%10==0:
        print("游戏失败！")
        break
    i = i + 1






