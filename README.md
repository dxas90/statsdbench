Benchmark of Go statsd clients

```
$ go test -bench . -benchmem -benchtime=5s
BenchmarkGoneS-4      	50000000	       213 ns/op	       0 B/op	       0 allocs/op
BenchmarkGoneP-4      	30000000	       200 ns/op	       0 B/op	       0 allocs/op
BenchmarkAlexcesaroS-4	10000000	       611 ns/op	       0 B/op	       0 allocs/op
BenchmarkAlexcesaroP-4	10000000	       648 ns/op	       0 B/op	       0 allocs/op
BenchmarkCactus-4     	 5000000	      1948 ns/op	       4 B/op	       0 allocs/op
BenchmarkG2s-4        	  500000	     14235 ns/op	     552 B/op	      23 allocs/op
BenchmarkQuipo-4      	 3000000	      2404 ns/op	     384 B/op	       7 allocs/op
```
