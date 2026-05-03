# Система мониторинга Zabbix. Часть 2 - Розаев А.Ю.

### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.

Желаем успехов в выполнении домашнего задания!
 
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

![Template](https://github.com/expgt/netzabbix2hw/blob/main/task1.png)

---

### Задание 2


---

### Задание 3

![Hosts](https://github.com/expgt/netzabbix2hw/blob/main/task2-3.png)

---

### Задание 4

![Dashboard](https://github.com/expgt/netzabbix2hw/blob/main/task4.png)

---

### Задание 5

![Map](https://github.com/expgt/netzabbix2hw/blob/main/task5.png)

---

### Задание 6

![Latest data bash](https://github.com/expgt/netzabbix2hw/blob/main/task6.png)

```bash
#!/bin/bash
if [ "$1" = 1 ]; then
   echo "Rozaev"
      exit 1
      
elif [ "$1" = 2 ]; then
    date
      exit 1
            
fi
```

---

### Задание 7

![Latest data python](https://github.com/expgt/netzabbix2hw/blob/main/task7.png)

```python
import sys
from datetime import datetime

now = datetime.now()
fnow = now.strftime("%d.%m.%Y %H:%M")

if (sys.argv[1] == '1'):
    print("Rozaev")
        
elif (sys.argv[1] == '2'):
    print(fnow)
                
else:
    print(f"unknown input: {sys.argv[1]}")
```

---

### Задание 8

![Discovery](https://github.com/expgt/netzabbix2hw/blob/main/task8_discovery.png)

![Rule](https://github.com/expgt/netzabbix2hw/blob/main/task8_rule.png)

---

### Задание 9

![Vagrantfile](https://github.com/expgt/netzabbix2hw/blob/main/Vagrantfile)

![zabbix-agent](https://github.com/expgt/netzabbix2hw/blob/main/zabbix-agent.sh)

---
