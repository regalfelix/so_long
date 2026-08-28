# so_long

A small 2D tile-based game built in C for 42, using [MLX42](https://github.com/codam-coding-college/MLX42) for graphics. Move a player around a map, collect all the items, and reach the exit in as few moves as possible.

## Technical overview

- C, MLX42 for windowing/rendering, custom `.ber` map files (ASCII grids: `1` wall, `0` floor, `P` player start, `C` collectible, `E` exit)
- Maps are validated on load: must be rectangular, fully enclosed by walls, and contain exactly one player, one exit, and at least one collectible
- Move count is tracked and printed to the terminal after every move

## Compile & run

```bash
git clone https://github.com/regalfelix/so_long.git
cd so_long
make
./so_long maps/map.ber
```

**Controls:** `W`/`A`/`S`/`D` to move, `Esc` to quit.

Several sample maps are included under `maps/`.

## License

This project is licensed under the [MIT LICENSE](LICENSE)
