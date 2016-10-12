Benchmark of my [StatsD client](https://github.com/alexcesaro/statsd) with the
Go clients listed on the
[StatsD wiki](https://github.com/etsy/statsd/wiki#client-implementations):

```
$ go test -bench . -benchmem -benchtime=5s
BenchmarkAlexcesaroS-4	20000000	       604 ns/op	       0 B/op	       0 allocs/op
BenchmarkAlexcesaroP-4	10000000	       681 ns/op	       0 B/op	       0 allocs/op
BenchmarkCactus-4     	 5000000	      1944 ns/op	       4 B/op	       0 allocs/op
BenchmarkG2s-4        	  500000	     15327 ns/op	     552 B/op	      23 allocs/op
BenchmarkQuipo-4      	 3000000	      2398 ns/op	     384 B/op	       7 allocs/op
```
