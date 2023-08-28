[home-url]: https://github.com/SotGE/Web-Run-Python 'Home'

---

# <p align="center">[Byndyusoft DevOps][home-url]</p>

<br/>

## Description

Для Byndyusoft на должность DevOps

<br/>

## Documentation

Устанавливаем на Windows 10/11:<br/>
WSL, Ubuntu, Docker, Kubernetes, Helm<br/>

Push себе на компьютер проект.<br/>
Переходим в директорию.<br/>
Устанавливаем/запускаем терминал Windows и выполняем дальнейшие действия.<br/>

Установка с пробным запуском и отладкой:<br/>
helm install . --name app --dry-run --debug<br/>

Смотрим статус релиза:<br/>
helm ls --all app<br/>

Смотрим список релизов с пространством имен:<br/>
helm list<br/>

Смотрим список деплойментов:<br/>
kubectl get deploy<br/>

Смотрим список подов:<br/>
kubectl get pods -o wide<br/>

Смотрим список сервисов:<br/>
kubectl get svc<br/>

Смотрим список обо всех сущностях во всех пространствах имен:<br/>
kubectl get all --all-namespaces=true<br/>

Проверим состояние ноды кластера этого приложения:<br/>
kubectl describe node app<br/>

Проверим состояние ноды кластера Kubernetes:<br/>
kubectl describe node kubernetes<br/>

Можем завершить обзор и удалить релиз:<br/>
helm delete app<br/>
или<br/>
helm uninstall app

<br/>

## System requirements

WSL, Ubuntu, Docker, Kubernetes, Helm

<br/>

## Contacts

Site: <https://sotge.ru/>

E-Mail: <sotge@hotmail.com>

Facebook: [@SotGEGDS](https://www.facebook.com/sotgegds 'https://www.facebook.com/sotgegds')

VK: [@SotGE](https://vk.com/sotge 'https://vk.com/sotge')

Twitter: [@SotGE](https://twitter.com/sotge 'https://twitter.com/sotge')

Telegram: [@SotGE](https://t.me/sotge 'https://t.me/sotge')
