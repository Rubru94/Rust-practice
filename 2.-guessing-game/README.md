# Guessing Game

Práctica del **capítulo 2** del libro [The Rust Programming Language Book](https://doc.rust-lang.org/book/title-page.html): el clásico juego de adivinar un número entre 1 y 100.

## Cómo ejecutar

```bash
cargo run
```

El programa genera un número secreto aleatorio y el jugador intenta adivinarlo. El programa responde con "Too small!", "Too big!" o "You win!" (y termina) cuando acierta.

## Qué enseña

- Entrada/salida por consola con `std::io`.
- Variables mutables e inmutables.
- Sombras (*shadowing*) de variables.
- Tipos: `String`, `u32`, `Ordering`.
- Control de flujo: `loop`, `break`, `continue`.
- `match` para comparar valores y para manejar errores de parseo.
- Crates externos y dependencias con Cargo (`rand`).

## Diferencias con el libro

- Se usa `rand::random_range(1..=100)` (API de `rand` 0.10) en lugar de `thread_rng().gen_range()`.
- La entrada no numérica no provoca un *panic*: se maneja con `match` mostrando `Invalid input. Try again.` y se sigue iterando.

## Dependencias

| Crate | Versión |
|-------|---------|
| [`rand`](https://crates.io/crates/rand) | 0.10.1 |