# @encoding/base64 — Base64 Encoding/Decoding for Zeta

Auto-converted from [base64](https://crates.io/crates/base64) v0.22.1 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **Engine API** — configurable encoding/decoding with pluggable engines
- **Standard** — RFC 4648 base64 with `=` padding
- **URL-safe** — RFC 4648 base64url (replaces `+/` with `-_`)
- **No-pad** — omits trailing `=` characters
- **Configurable alphabets** — custom character sets
- **Display** — `Display` trait for non-allocating formatting

## Usage
```zeta
use @encoding/base64::{Engine, engine::general_purpose};

let encoded = general_purpose::STANDARD.encode(b"hello world");
let decoded = general_purpose::STANDARD.decode(&encoded).unwrap();
```

## Stats: ~2,634 lines, 0 unsupported items

## License: MIT