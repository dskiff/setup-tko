# setup-tko

A simple setup action for [tko](https://github.com/dskiff/tko).

```
# ... perform build and place output in ./out ...

- use: dskiff/setup-tko@main

- name: Publish
  run: tko "./out"
  env:
    TKO_BASE_IMAGE: debian:bookworm-slim@sha256:155280b00ee0133250f7159b567a07d7cd03b1645714c3a7458b2287b0ca83cb
    GITHUB_TOKEN: ${{ github.token }}
```
