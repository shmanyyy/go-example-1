package main

import "fmt"

func makeCounter() func() int {
 count := 0
 return func() int {
  count++
  return count
 }
}
func main() {
 fmt.Println("Start of the programm")
 counter := makeCounter()

 for i := 1; i <= 10; i++ {
  result := counter()
  fmt.Println(result)

  if result > 5 {
   fmt.Println("Break")
   break
  }
 }

 fmt.Println("End of the program")
}
