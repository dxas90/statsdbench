Benchmark of my [StatsD client](https://github.com/alexcesaro/statsd) with the
Go clients listed on the
[StatsD wiki](https://github.com/etsy/statsd/wiki#client-implementations):

```
$ go test -bench . -benchmem -benchtime=5s
BenchmarkAlexcesaro-4	10000000	       619 ns/op	       0 B/op	       0 allocs/op
BenchmarkCactus-4    	 5000000	      1921 ns/op	       4 B/op	       0 allocs/op
BenchmarkG2s-4       	  500000	     14931 ns/op	     552 B/op	      23 allocs/op
BenchmarkQuipo-4     	 3000000	      2372 ns/op	     384 B/op	       7 allocs/op
```
