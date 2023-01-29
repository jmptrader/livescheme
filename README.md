# Building a Scheme-like language in Golang live on Twitch

Requirements:
* Go 1.18+

To run:

```shell
$ go mod tidy
$ go test
$ go build
$ cat examples/fib.scm
(func fib (a)
      (if (< a 2)
	  a
	  (+ (fib (- a 1)) (fib (- a 2)))))

(fib 11)
$ ./livescheme examples/fib.scm
89
```

Stream:
* Sundays at 5pm NY time
* [https://twitch.tv/eatonphil](twitch.tv/eatonphil)

Archives:
* [Part 1: A lexer](https://www.youtube.com/watch?v=lZNhZI-dN9k)
* [Part 2: Parsing](https://www.youtube.com/watch?v=5ttFEPQopXc)
* [Part 3: AST walking interpreter](https://www.youtube.com/watch?v=YwmGcverSHI)
