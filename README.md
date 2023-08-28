[home-url]: https://github.com/SotGE/Byndyusoft-DevOps 'Home'

---

# <p align="center">[Byndyusoft DevOps][home-url]</p>

<br/>

## Description

Для Byndyusoft на должность DevOps

<br/>

## Documentation

Устанавливаем на Windows 10/11:<br/>
WSL-Ubuntu-Docker Desktop, Kubernetes, Helm<br/>

При двухсторонней связке, проект можем тестировать как на Linux, так и на Windows в единой среде, через настроенный Visual Studio Code (для этого нужнго будет установить плагины extension pack Remote Development, Docker, Kubernetes).

- Git Clone себе на компьютер этот проект.<br/>
- Переходим в директорию.<br/>
- Устанавливаем/запускаем терминал Windows и выполняем дальнейшие действия.<br/>

Установка:<br/>

- helm install app .<br/>

Смотрим список релизов с пространством имен:<br/>

- helm ls --all<br/>
  или
- helm list<br/>

Смотрим список деплойментов:<br/>

- kubectl get deploy<br/>

Смотрим список подов:<br/>

- kubectl get pods -o wide<br/>

Смотрим список сервисов:<br/>

- kubectl get svc<br/>

Смотрим список обо всех сущностях во всех пространствах имен:<br/>

- kubectl get all --all-namespaces=true<br/>

Смотрим информацию о кластере:<br/>

- kubectl cluster-info<br/>

Смотрим описание сервиса этого приложения:<br/>

- kubectl describe services service-app-helm<br/>

Смотрим описание сервиса Kubernetes:<br/>

- kubectl describe services kubernetes<br/>

Можем завершить обзор и очистить релиз:<br/>

- kubectl delete services service-app-helm
- kubectl delete deployment deployment-app-helm-app

Можем завершить обзор и удалить релиз:<br/>

- helm delete app<br/>
  или<br/>
- helm uninstall app

<br/>

## System requirements

- Windows 10/11 (можно сразу на Linux/Mac все настроить);<br/>
- WSL-Ubuntu-Docker Desktop;<br/>
- Kubernetes;<br/>
- Helm (можно через choco установить).

<br/>

## Contacts

Maksim E. Sorokin

E-Mail: <sotge@hotmail.com>

Facebook: [@SotGEGDS](https://www.facebook.com/sotgegds 'https://www.facebook.com/sotgegds')

VK: [@SotGE](https://vk.com/sotge 'https://vk.com/sotge')

Twitter: [@SotGE](https://twitter.com/sotge 'https://twitter.com/sotge')

Telegram: [@SotGE](https://t.me/sotge 'https://t.me/sotge')
