代码开启pprof
```
import _ "net/http/pprof"

func main() {
    go func() {
        log.Println(http.ListenAndServe("localhost:6060", nil))
    }()
    // 其他业务代码...
}
```

curl http://localhost:6060/debug/pprof/goroutine -o goroutine.txt
curl http://localhost:6060/debug/pprof/heap -o heap.pprof