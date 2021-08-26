package main

import (
	"flag"
	"fmt"
)

var (
	t int
)

func main() {
	flag.IntVar(&t, "type", 3, "显示唐诗宋词")
	flag.Parse()

	// fmt.Println(t)

	if t == 1 {
		fmt.Println("唐诗")
	} else {
		fmt.Println("宋词")
	}

}
