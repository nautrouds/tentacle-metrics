# tentacle-metrics

This repository provides shared Protocol Buffer definitions for metric data, facilitating communication between services.

## Rust Usage

To use this library in a Rust project, add it to your `Cargo.toml`:

```toml
[dependencies]
tentacle-metrics = { git = "https://github.com/nautrouds/tentacle-metrics.git", branch = "main" }
```

You can access the generated protobuf types under the `pb` module:

```rust
use tentacle_metrics::pb::MetricPayload;
```

## Go Usage

Since this repository contains a `go.mod` file and is structured for Go modules, you can import it directly into your Go projects:

```go
import (
    "github.com/nautrouds/tentacle-metrics/pb"
)

// Example usage:
func main() {
    payload := &pb.MetricPayload{
        TentacleId: "instance-01",
        Service:    "proxy-service",
    }
}
```

Ensure you run `go get github.com/nautrouds/tentacle-metrics` in your project directory to fetch the dependency.
