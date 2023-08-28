[home-url]: https://github.com/SotGE/Web-Run-Python 'Home'

---

# <p align="center">[Byndyusoft DevOps][home-url]</p>

<br/>

## Description

Для Byndyusoft на должность DevOps

<br/>

## Documentation

Устанавливаем на Windows 10/11:
WSL, Ubuntu, Docker, Kubernetes, Helm

Push себе на компьютер проект.
Переходим в директорию.
Устанавливаем/запускаем терминал Windows и выполняем дальнейшие действия.

Установка с пробным запуском и отладкой:
helm install . --name app --dry-run --debug

Смотрим статус релиза:
helm ls --all app

Смотрим список релизов с пространством имен:
helm list

Смотрим список деплойментов:
kubectl get deploy

Смотрим список подов:
kubectl get pods -o wide

Смотрим список сервисов:
kubectl get svc

Смотрим список обо всех сущностях во всех пространствах имен:
kubectl get all --all-namespaces=true

Проверим состояние ноды кластера этого приложения:
kubectl describe node app

Проверим состояние ноды кластера Kubernetes:
kubectl describe node kubernetes

Можем завершить обзор и удалить релиз:
helm delete app
или
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
