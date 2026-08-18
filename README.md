# Система онлайн-заказа товаров

## О проекте

Учебный проект по системному анализу процесса оформления
и обработки интернет-заказа.

## Цель

Спроектировать целевой бизнес-процесс и системное
взаимодействие компонентов.
В рамках проекта рассматриваются Use Case:

- просмотр каталога;
- создание заказа;
- проверка наличия товара;
- проверка статуса заказа;
- добавить товар в корзину;
- резервирование товара;
- оплата;
- отмена заказа;
- передача на сборку;
- сборка заказа.

## Требования
[Открыть Функциональные требования](FunctionalRequirments.md)

[Открыть Нефункциональные требования](NonFunctionalRequirements.md)

## Диаграммы

### BPMN

<img width="1841" height="1295" alt="image" src="https://github.com/user-attachments/assets/c41eac43-f63c-4442-a1c3-99d4bcb06ddb" />


### Use Case

[Открыть Use Case](UseCase.puml)

<img width="958" height="1050" alt="image" src="https://github.com/user-attachments/assets/eb254bce-cead-4149-9399-94ac195fc302" />

### Sequence

[Открыть Sequence Diagram](SequenceDiagram)

<img width="1164" height="1960" alt="image" src="https://github.com/user-attachments/assets/b7690c3a-f14b-4531-9548-c8de9b7ef313" />


### Class Diagram

[Открыть Class Diagram](ClassDiagram)

<img width="717" height="697" alt="image" src="https://github.com/user-attachments/assets/5498698a-34fb-445c-8453-9f9909ac5532" />


### API
Получение заказа:

GET /api/v1/orders/{orderId}

Оплата:

POST /api/v1/orders/{orderId}/payment

Отмена:

POST /api/v1/orders/{orderId}/cancel

Статус:

GET /api/v1/orders/{orderId}/status

OpenAPI specification:

[openapi.yaml](openapi.yaml)

### Коды
201 Created
400 Bad Request
404 Not Found
422 Unprocessable Content
500 Internal Server Error
