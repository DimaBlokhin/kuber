# kuber
Пример проекта, в котором я создаю простое веб-приложение, упаковываю его в контейнер Docker, а затем запускаю эти контейнеры с помощью Kubernetes.



# Контейнеризация и Оркестрация с использованием Docker и Kubernetes

Этот проект представляет собой пример контейнеризации веб-приложения с использованием Docker и его оркестрации с помощью Kubernetes.

## Шаги по созданию проекта

### 1. Создание веб-приложения

### 2. Контейнеризация приложения с Docker

#### Создание Docker-образа

```docker build -t webApp . ```

```docker run -p 5000:5000 webApp```

#### Приложение должно быть доступно по адресу http://localhost:5000

### 3. Работа с Kubernetes

#### Установка Minikube
#### Следуйте инструкциям для установки Minikube.
#### Запуск Minikube

```minikube start```

#### Применение конфигураций Kubernetes

```kubectl apply -f deployment.yml```
```kubectl apply -f service.yml```

### 4. Тестирование развертывания

#### Получение IP-адреса Minikube

```minikube ip```

#### Откройте веб-браузер по адресу http://<minikube_ip>:<service_port>
