FROM caddy:2.3.0-builder AS builder

RUN xcaddy build --with github.com/caddy-dns/cloudflare

FROM caddy

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
