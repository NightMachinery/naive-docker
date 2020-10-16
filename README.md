# Naïve Docker

Run [NaïveProxy](https://github.com/klzgrad/naiveproxy) in Docker.

## Usage

- Change parts marked with `CHANGEME` appropriately in the [Caddyfile](config/Caddyfile)
- Build the image with `docker build -t naive .`
- Start with `docker-compose up [-d]`

### Client

Install [`naive`](https://github.com/klzgrad/naiveproxy) on the client and run:

``` sh
naive --listen="socks://127.0.0.1:1080" --proxy='https://user:pass@example.com' --log
```

This will give you a socks5 proxy on localhost:1080.
