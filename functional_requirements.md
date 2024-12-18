<h1 style="text-align:center">Код Use-Case диаграммы рисунка 1</h1>

```uml

@startuml

actor "Клиент" as fc

left to right direction

rectangle "Мойка.ру"  {
  usecase "UC1: Записаться на мойку" as UC1
	usecase "UC1.1: Найти и выбрать автомойку" as UC2
	usecase "UC1.2: Выбрать дату и время" as UC3
	usecase "UC1.3: Выбрать услугу" as UC4
	usecase "UC2: Отменить услугу" as UC5
	usecase "UC1.4: Оплатить" as UC6
}

UC1 --> UC2:(include)
UC1 --> UC3:(include)
UC1 --> UC4:(include)
UC1 ..> UC6:(exclude)

fc --> UC1
fc --> UC5


@enduml

```
