package main

import (
 "fmt"
)

// Person структура, представляющая человека
type Person struct {
 Name     string // Имя человека
 Age      int    // Возраст человека
 HeightCM float64 // Рост человека в сантиметрах
}

// Walk метод, который имитирует ходьбу человека
func (p  * Person) Walk() {
 fmt.Println("Walking...")
}

// Eat метод, который имитирует прием пищи человеком
func (p  * Person) Eat(foodType string) {
 fmt.Printf("Eating %s...\n", foodType)
}

// Think метод, который имитирует мыслительный процесс человека
func (p  * Person) Think() {
 fmt.Println("Thinking...")
}

// InterfacePerson интерфейс, которому соответствует тип Person
type InterfacePerson interface {
 Walk()
 Eat(foodType string)
 Think()
}

// Programmer структура, представляющая программиста
type Programmer struct {
 Person
 Languages []string // Языки программирования, которыми владеет программист
}

// Code метод, который имитирует написание кода программистом
func (p  * Programmer) Code(language string) {
 fmt.Printf("Coding in %s...\n", language)
}

// InterfaceProgrammer интерфейс, которому соответствует тип Programmer
type InterfaceProgrammer interface {
 Code(language string)
}

func main() {
 // Создание переменных для типов Person и Programmer
 person := Person{
  Name:     "John",
  Age:      30,
  HeightCM: 180,
 }
 programmer := Programmer{
  Person: person,
  Languages: []string{
   "Go",
   "JavaScript",
  },
 }

 // Вызов методов типа Person из переменной programmer
 person.Walk()
 person.Eat("pizza")
 person.Think()

 // Вызов методов типа Programmer из переменной programmer
 programmer.Code("Go")
}
