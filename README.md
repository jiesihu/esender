# esender
## Introduction
This package is developed based on yagmail and is used to send messages using 163 e-mail, so you have to own a 163 account first :-). Personaly, I use it to send deep learning progress to my mailbox. (Significantly reduced my anxiety)  

## Notes for mail 163 
Usually, you need to turn on the IMAP/SMTP service of your account manually. That is free. It will generate an authorization password which is exactly the input password in the example below. Note that you don't need the password of your account to send the e-mail.

## Usage

### Scenario 1
Send a email directly with function 'Esender'

Example:
```
from esender import Esender

Esender(user = 'your163account@163.com',  password='****',to = ['yourtargetemail@qq.com'],\
    subject = 'Subject',content = 'your content', attachment = './hello.txt')
```
### Scenario 2
Monitor the time consuming of a your task and send emails when the it ends.  

Example:
```
from esender import time_counter
@time_counter(user = 'your163account@163.com',  password='***',to = ['yourtargetemail@qq.com'],\
    subject = 'Subject',content = 'Your content', attachment = None)
def main():
    return ...

main()
```

# To do
- [ ] Add help()  
- [ ] Works with more e-mail