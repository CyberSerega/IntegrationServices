<h1 style="text-align:center">Код Use-Case диаграммы рисунка 1</h1>

```uml

@startuml

actor "Клиент" as fc

left to right direction

rectangle "Мойка.ру"  {
	usecase "Поиск автомойки" as UC1
	usecase "Выбрать мойку" as UC2
	usecase "Выбрать дату и время" as UC3
	usecase "Выбрать услугу" as UC4
	usecase "Отменить услугу" as UC5
	usecase "Оплатить" as UC6
}



fc --> UC1
fc --> UC2
fc --> UC3
fc --> UC4
fc --> UC5
fc --> UC6

@enduml

```
