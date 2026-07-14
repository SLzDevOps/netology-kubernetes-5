# Домашнее задание "Хранение в K8s" - `Фомичев Анатолий`

## Ссылка на Д3 - https://github.com/netology-code/kuber-homeworks/blob/shkuber-16/2.1/2.1.md

## Ссылка на репозиторий - 


### Задача 1

#### манифест .yaml
https://github.com/SLzDevOps/netology-kubernetes-5/tree/main/task1
   
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_993.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1006.png).
      
    
### Задача 2
  
#### манифест .yaml
https://github.com/SLzDevOps/netology-kubernetes-5/tree/main/task2
    
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_998.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_999.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1002.png).
  
  После удаления PVC, PV, который был с ним связан, переходит в состояние Released. Это означает, что привязка между PV и PVC разорвана, но данные на хранилище сохраняются, так как политика восстановления (Reclaim Policy) установлена в значение Retain. Эта политика предотвращает автоматическое удаление данных, позволяя администратору вручную проверить их и принять решение о дальнейшем использовании.
  
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1003.png).
  
  PV создан с типом hostPath, который монтирует реальную директорию на ноде (/mnt/data-exchange). Данные, записанные в эту директорию, не зависят от жизненного цикла Kubernetes-объектов. Даже после удаления PVC и Deployment, физические файлы на ноде остаются нетронутыми, так как они находятся вне управления Kubernetes.
  PV — это только API-объект в Kubernetes, описывающий хранилище. Удаление PV не влияет на физические файлы на ноде, так как они не управляются Kubernetes напрямую. Для типа hostPath удаление PV просто удаляет описание из API, не затрагивая реальные данные на диске. Данные могут быть удалены только вручную администратором.




### Задача 3
  
#### манифест .yaml
https://github.com/SLzDevOps/netology-kubernetes-5/tree/main/task3
  
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_993.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1006.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_993.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1006.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_993.png).
![alt text](https://github.com/SLzDevOps/netology-kubernetes-5/blob/main/screenshots/Screenshot_1006.png).
