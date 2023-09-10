# Nestjs Express vs Bun(Express)

## Installation

```bash
$ bun install # doesn't effect node performance
```

## Running the app

```bash
# development mode
$ npm run start:dev
$ bun run start:bun

# production mode
$ npm run start:prod
$ bun run start:prod:bun
```
# Benchmarks
* __Machine:__ `Apple 14" M2 Pro | Apple M2 Pro 10-Core CPU | 16GB.`
* __Node:__ `v18.14.0`
* __Run:__ `Sun Sep 10 10:31:11 +03 2023`

|                     | Router | Requests/s | Latency | Throughput/Mb |
|:--------------------| --:    | :-:        | --:     | --:           |
| nestjs-express      | ✓      | 16874.41    | 116.9 ms    | 4.03 MB          |
| bun(nestjs-express) | ✓      | 41212.81    | 47.88 ms    | 7.91 MB          |
For testing locally:
```bash
$ npm run benchmark
$ bun run benchmark:bun
```
Somehow process stales in background, so you need to kill it manually.

## License

Nest is [MIT licensed](LICENSE).
