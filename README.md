# Homework_week8

## 一、使用 redis benchmark 工具, 测试 10 20 50 100 200 1k 5k 字节 value 大小，redis get set 性能。



### 1、redis-benchmark -d 10000 -t SET,GET

Set:

```shell
Summary:
  throughput summary: 143266.47 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.215     0.080     0.191     0.327     0.943     9.527
```

Get:

```shell
Summary:
  throughput summary: 151057.41 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.191     0.080     0.183     0.247     0.447     1.015
```

### 2、redis-benchmark -d 5000 -t SET,GET

Set:

```shell
Summary:
  throughput summary: 146842.88 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.205     0.088     0.175     0.327     0.991     5.183
```

Get:

```shell
Summary:
  throughput summary: 157480.31 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.183     0.080     0.175     0.255     0.439     1.191
```

### 2、redis-benchmark -d 1000 -t SET,GET

Set:

```shell
Summary:
  throughput summary: 141643.06 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.226     0.064     0.167     0.487     1.303     3.151
```

Get:

```shell
Summary:
  throughput summary: 152207.00 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.193     0.096     0.167     0.343     0.479     0.711
```

### 2、redis-benchmark -d 200 -t SET,GET

Set:

```shell
Summary:
Summary:
  throughput summary: 156985.86 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.189     0.080     0.167     0.303     0.583     7.095
```

Get:

```shell
Summary:
  throughput summary: 157480.31 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.189     0.072     0.167     0.351     0.511     0.743
```

### 2、redis-benchmark -d 100 -t SET,GET

Set:

```shell
Summary:
  throughput summary: 155279.50 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.196     0.080     0.167     0.343     1.159     3.167
```

Get:

```shell
Summary:
  throughput summary: 169491.53 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.170     0.056     0.159     0.239     0.415     0.863
```

### 2、redis-benchmark -d 50 -t SET,GET

Set:

```shell
Summary:
  throughput summary: 155038.77 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.199     0.072     0.167     0.343     1.319     5.031
```

Get:

```shell
Summary:
  throughput summary: 168634.06 requests per second
  latency summary (msec):
          avg       min       p50       p95       p99       max
        0.171     0.056     0.159     0.255     0.407     0.879
```

### 
