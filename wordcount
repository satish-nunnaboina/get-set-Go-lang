package main

import (
	"golang.org/x/tour/wc"
	"strings"
)

func WordCount(s string) map[string]int {
	m := make(map[string]int)
	words := strings.Fields(s)
	for i := range words{
		v, ok := m[words[i]]
		switch ok {
			case false: m[words[i]] = 1
			case true: m[words[i]] = v + 1
		}
	}
	
	return m
}

func main() {
	wc.Test(WordCount)
}
