
package main

import "fmt"

func main() {
	//keepGoing("heyyy", 5)
	var w Writer = ConsoleWriter{}
	w.Write([]byte("Hello Go !"))

	var w1 Writer = ConsoleWriter1{}
	w1.Write([]byte("Hello Go !"))

}

type Writer interface {
	Write([]byte) (int, error)
}

type ConsoleWriter struct{}

type ConsoleWriter1 struct{}

func (cw ConsoleWriter) Write(data []byte) (int, error) {
	n, err := fmt.Println(string(data))
	return n, err
}

func (cw ConsoleWriter1) Write(data []byte) (int, error) {
	n, err := fmt.Println(string(data))
	return n, err
}
