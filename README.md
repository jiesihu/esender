# esender
## Introduction
This package is developed based on yagmail and is used to send messages using 163 e-mail, so you have to own a 163 account first :-). Personaly, I use it to send deep learning progress to my mailbox. (Significantly reduced my anxiety)  

## Usage
### scenario 1
```
from esender import time_counter
@time_counter(user = 'jiesihu*****@163.com',  password='***',to = ['******@qq.com'],subject = 'Training',content = 'Hi mac', attachment = None)
def your_main():
    return ...

your_main()
```
### scenario 2
```
from esender import Esender

Esender(user = 'jiesihu002@163.com',  password='****',to = ['******@qq.com'],subject = 'Training',content = 'Hi mac2', attachment = None)
```
    