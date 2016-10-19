# OOAD-WEEK09
##Class Diagram


###Class Diagram1
code 
'''
@startuml
title Classes - Class Diagram
class Customer {
  +FirstName
  +LastName
  +CardName
  +PinNumber
  +Account
  -VerifyPassword()
}
class Account {
  +Number
  +LastName
  +Balance
  +Transaction
  -Deposit()
  -Withdraw()
  -UpdateAccount()
  }  
class Transaction {
  +TransactionID
  +TransactionDate
  +TransactionTime
  +TransactionType
  +Account
  +Amount
  +PostBalance
  }
Left to Right direction
class Customer -- Class Account: has
class Account -- Class Transaction: Perfrom
@enduml
'''
diagram


<img src="https://github.com/NATAKORNCHA/OOAD-WEEK09/blob/master/Homework/Class%20Diagram1.png?raw=true">



###Class Diagram2
code 
'''
@startuml
title Class <b>People </b>
People  <.. SomChai:Is member of
People  <.. SomJit:Is member of
People  <.. SomRuk:Is member of
People  <.. SomJai:Is member of
@enduml
'''
diagram
<img src="https://github.com/NATAKORNCHA/OOAD-WEEK09/blob/master/Homework/Class%20Diagram2.png?raw=true">


###Class Diagram3
code 

'''
@startuml
title Class <b>CAR </b>
Car  <.. BMW:Is member of
Car  <.. HONDA:Is member of
Car  <.. Ferrari:Is member of
Car  <.. Benz:Is member of
@enduml
'''

diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK09/blob/master/Homework/Class%20Diagram3.png?raw=true">


###Class Diagram4
code 

'''
@startuml
class Flight {
   flightNumber : Integer
   departureTime : Date
   flightDuration : Minutes
   DelayFlight (numberOfminuestes :int) :Data
   getArrivalTime(): Date
}
@enduml
'''

diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK09/blob/master/Homework/Class%20Diagram4.png?raw=true">


###Class Diagram5
code 

'''
@startuml
class Car

Driver - Car : drives >
Car *- Wheel : have 4 >
Car -- Person : < owns

@enduml
'''

diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK09/blob/master/Homework/Class%20Diagram5.png?raw=true">



