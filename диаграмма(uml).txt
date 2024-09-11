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
rectangle "Платежная система" {
  usecase "Наличный расчет" as PS1
  usecase "Безналичный расчет" as PS2
}


fc --> UC1
fc --> UC2
fc --> UC3
fc --> UC4
fc --> UC5
fc --> UC6
UC6 <-- PS1
UC6 <-- PS2

@enduml
