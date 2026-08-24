# haepari-supply

Public, signed official asset supply for Haepari Antarctic distribution.

- Official index: `official/index.json`
- Detached index signature: `official/index.signature.json`
- Trust metadata: `official/trust.json`
- Packages: `official/packages/<asset-id>/<version>/`

The Haepari desktop app embeds the Ed25519 public key from `trust.json`. It verifies the exact index and
manifest bytes, every package hash, and every extracted file before accepting an asset into its isolated
official cache. Files in this repository are public distribution artifacts; the signing private key is never
committed here.

해파리 앱은 색인·manifest의 받은 바이트와 각 압축 꾸러미·파일의 해시를 모두 검증합니다.
받은 공식판은 사용자 바다의 `양식/`·`틀/`을 자동으로 덮어쓰지 않습니다.
