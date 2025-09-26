# PixcelGuard SFML

Repo mẫu để chạy game PixcelGuard trên GitHub Pages bằng Emscripten.

## Cấu trúc
- `PixcelGuardSFML.cpp`: mã nguồn game (SFML)
- `assets/`: thư mục ảnh
- `index.html`: file HTML để load game
- `index.js` + `index.wasm`: sinh ra khi build bằng Emscripten

## Cách build bằng Emscripten
```bash
emcc PixcelGuardSFML.cpp -o index.html -s USE_SDL=2 -s USE_SFML=2 -s WASM=1
```
