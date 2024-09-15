# Fuzzing

```sh
# Run test without fuzzing it to make sure the seed inputs pass.
go test
```

```sh
# Run test with fuzzing,
# to see if any randomly generated string inputs will cause a failure
go test -fuzz=Fuzz
```

```sh
# Fuzz with `-fuzztime` will fuzz for 30 seconds
# before exiting if no failure was found
go test -fuzz=Fuzz -fuzztime 30s
```
