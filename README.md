# HOMEWORK #40

## Создал сеть, подсеть и ВМ из модуля /modules/yandex_vm

![alt text](HW_PIC/1.png)
![alt text](HW_PIC/2.png)

## Создал сервисный аккаунт, предоставил ему права, создал для него ключ и создал S3 хранилище для хранения состояний terraform из директории setup_backend

![alt text](HW_PIC/3.png)
![alt text](HW_PIC/4.png)
![alt text](HW_PIC/5.png)

## Мигрировал хранение состояния terraform с ключем -migrate-state в S3 хранилище

![alt text](HW_PIC/6.png)
![alt text](HW_PIC/7.png)

## Добавил в terraform security_group и в модуль создания ВМ добавил зависимость 'depends_on = [ yandex_vpc_security_group.web_sg ]', явно указав, чтобы ВМ создавалась только после сооздания security_group

![alt text](HW_PIC/8.png)

## ВМ создалась только после security_group