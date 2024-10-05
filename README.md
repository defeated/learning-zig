# learning zig

## resources

1. https://ziglang.org
2. https://zig.guide

## commands

```
zig run src/main.zig
```
```
zig test test/test_pass.zig
```
```
zig test test/test_fail.zig
```
```
zig build-exe src/main.zig -O ReleaseSmall -fstrip -fsingle-threaded -femit-bin=zig-out/main
```
```
zig build
./zig-out/bin/learning-zig
```
