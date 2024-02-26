### Info atom ('info')

An atom that defines a single track of a info.  
Same as [trak atom](https://developer.apple.com/documentation/quicktime-file-format/track_atom).

#### Writing to [mdat atom](https://developer.apple.com/documentation/quicktime-file-format/movie_data_atom).

| bytes | description |
| ---- | ---- |
| 4 | info size (decompressed) |
| 4 | 'zstd' |
| variable | zstd compressed info |

#### info

Format similar to [glb](https://github.com/KhronosGroup/glTF).  
⚠️ Use offset/length key instead of byteOffset/byteLength.

| bytes | description |
| ---- | ---- |
| 4 | JSON size |
| 4 | 'JSON' |
| variable | Structured JSON content |
| 4 | BIN size |
| 4 | 'BIN ' |
| variable | Binary buffer |