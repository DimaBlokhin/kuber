# kuber
Example of the project, where i'm gonna whip up a simple web app, pack it into a Docker container, and then run these containers using Kubernetes



# Контейнеризация и Оркестрация с использованием Docker и Kubernetes

Этот проект представляет собой пример контейнеризации веб-приложения с использованием Docker и его оркестрации с помощью Kubernetes.

## Шаги по созданию проекта

### 1. Создание веб-приложения

### 2. Контейнеризация приложения с Docker

#### Создание Docker-образа

```bash
docker build -t webApp .

#### Тестирование контейнера локально

docker run -p 5000:5000 webApp

#### Приложение должно быть доступно по адресу http://localhost:5000

### 3. Работа с Kubernetes

#### Установка Minikube
#### Следуйте инструкциям для установки Minikube.
#### Запуск Minikube

minikube start

#### Применение конфигураций Kubernetes

kubectl apply -f deployment.yml
kubectl apply -f service.yml

### 4. Тестирование развертывания

#### Получение IP-адреса Minikube

minikube ip

#### Откройте веб-браузер по адресу http://<minikube_ip>:<service_port>








