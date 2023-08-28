[home-url]: https://github.com/SotGE/Byndyusoft-DevOps 'Home'
[img1]: ./.gitimg/1.jpg 'Скриншот 1'
[img2]: ./.gitimg/2.jpg 'Скриншот 2'
[checklist]: ./CHECKLIST.md 'CHECKLIST'

---

# <p align="center">[Byndyusoft DevOps][home-url]</p>

### **<p align="center">[Посмотреть чек-лист >>][checklist]</p>**

<br/>

## Description

### Для Byndyusoft на должность DevOps

Перед запуском проекта на проду, проверим 👉 [чек-лист][checklist]

<br/>

## Documentation

Устанавливаем на Windows 10/11:<br/>
WSL-Ubuntu-Docker Desktop, Kubernetes, Helm<br/>

Проверяем, чтобы в C:\Windows\System32\drivers\etc\hosts записалась информация при установке ПО.<br/>

Пример:<br/>
\# Added by Docker Desktop<br/>
192.168.1.102 host.docker.internal<br/>
192.168.1.102 gateway.docker.internal<br/>
\# To allow the same kube context to work on the host and the container:<br/>
127.0.0.1 kubernetes.docker.internal<br/>
\# End of section<br/>

IP в hosts нужны для подключения к микросервису из localhost, если потребуется запуск не в проде.<br/>

При двухсторонней связке, проект можем тестировать как на Linux, так и на Windows в единой среде, через настроенный Visual Studio Code (для этого нужнго будет установить плагины "extension pack Remote Development", "Docker", "Kubernetes").<br/>

- Git Clone себе на компьютер этот проект;<br/>
- Перебрасываем проект в WSL-Ubuntu (\\wsl.localhost\Ubuntu\home\<имя компьютера>), фактически мы перебросили проект на продакшен (аналогично можно было бы перебросить в Azure, AWS, GCC и т.п. через настроенный ssh терминал+токен);<br/>
- Устанавливаем/запускаем проект в VSCode (предварительно подключаемся к WSL-Ubuntu, через плагин WSL, то есть в VSCode нажимаем комбинацию Ctrl+Shift+P пишем WSL: Connect to WSL using Distro in New Window... и подключаемся к Ubuntu);<br/>
- Смотрим в терминале текущий путь, прописав "pwd";<br/>
- Переходим в директорию (cd /home/<имя компьютера>/app);<br/>
- Смотрим наличие файлов проекта, пишем в терминале "ls" и в VSCode выбираем путь к проекту (лучше использовать плагин Remote Explorer или установить весь пакет "extension pack Remote Development"). Выполняем дальнейшие действия.<br/>

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

Получаем IP-адрес основной системы, выполнив следующую команду из дистрибутива Linux:<br/>

- Вводим: cat /etc/resolv.conf<br/>
- Скопировать IP-адрес в строке, начинающейся с nameserver<br/>
- Подключаемся к серверу WSL-Ubuntu, используя скопированный IP-адрес<br/>

Пример:<br/>
http://172.18.160.1<br/>

##### <p align="center">![img1]</p>

## Результат запущенного приложения в продакшене:

##### <p align="center">![img2]</p>

Можем завершить обзор и очистить релиз:<br/>

- kubectl delete services service-app-helm<br/>
- kubectl delete deployment deployment-app-helm-app<br/>

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
