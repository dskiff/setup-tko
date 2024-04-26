# setup-tko

A simple setup action for [tko](https://github.com/dskiff/tko).

```
# ... perform build and place output in ./out ...

- use: dskiff/setup-tko@main

- name: Publish
  run: tko build "./out"
  env:
    GITHUB_TOKEN: ${{ github.token }}
```
