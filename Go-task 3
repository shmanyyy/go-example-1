package main

import (
    "fmt"
)

type MyStruct struct {
    name string
}

func normalFuncSlice(slice []int) {
    for i := range slice {
        slice[i] = 2
    }
}

func pointerFuncSlice(slice []int) {
    for i := range slice {
        (slice)[i] = 2
    }
}

func normalFuncArray(arr [5]int) {
    for i := range arr {
        arr[i] = 2
    }
}

func pointerFuncArray(arr [5]int) {
    for i := range arr {
        (arr)[i] = 2
    }
}

func normalFuncMap(m map[string]int) {
    for key := range m {
        m[key] = 2
    }
}

func pointerFuncMap(m map[string]int) {
    for key := range m {
        (m)[key] = 2
    }
}

func normalFuncStruct(s MyStruct) {
    s.name += " Updated"
}

func pointerFuncStruct(s MyStruct) {
    s.name += " Updated"
}

func main() {
    // Слайс
    slice := []int{1, 2, 3, 4, 5}
    normalFuncSlice(slice)
    fmt.Println("Slice after normal function:", slice)

    slicePointer := []int{1, 2, 3, 4, 5}
    pointerFuncSlice(&slicePointer)
    fmt.Println("Slice after pointer function:", slicePointer)

    // Массив
    array := [5]int{1, 2, 3, 4, 5}
    normalFuncArray(array)
    fmt.Println("Array after normal function:", array)

    arrayPointer := [5]int{1, 2, 3, 4, 5}
    pointerFuncArray(&arrayPointer)
    fmt.Println("Array after pointer function:", arrayPointer)

    // Мапа
    m := map[string]int{"a": 1, "b": 2, "c": 3}
    normalFuncMap(m)
    fmt.Println("Map after normal function:", m)

    mPointer := map[string]int{"a": 1, "b": 2, "c": 3}
    pointerFuncMap(&mPointer)
    fmt.Println("Map after pointer function:", mPointer)

    // Структура
    myStruct := MyStruct{name: "John"}
    normalFuncStruct(myStruct)
    fmt.Println("Struct after normal function:", myStruct)

    myStructPointer := &MyStruct{name: "John"}
    pointerFuncStruct(myStructPointer)
    fmt.Println("Struct after pointer function:", myStructPointer)
}
