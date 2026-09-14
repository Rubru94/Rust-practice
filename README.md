# Rust Practice

Espacio de trabajo para prácticas de [**Rust**](https://rust-lang.org/es/) siguiendo la documentación oficial: [The Rust Programming Language Book](https://doc.rust-lang.org/book/title-page.html).

## Propósito

Cada concepto o capítulo del libro se practica en un **repo de Git independiente**, lo que permite:

- Aislar cada práctica y su evolución.
- Historial de commits limpio y enfocado por tema.
- Comparar enfoques entre ejercicios.
- Caso de estudio: [`hello-world`](hello-world/) — primer programa, "Hello world!".

## Estructura

```
Rust-practice/
├── hello-world/          # Práctica: Hello World (capítulos 1-2)
├── <tema>/               # Próximas prácticas, cada una con su propio repo Git
└── README.md             # Este archivo
```

## Cómo crear una nueva práctica

```bash
cargo new <nombre-de-la-practica>
```

Inicializar como repo Git propio (si `cargo new` no lo creó):

```bash
cd <nombre-de-la-practica>
git init
```

## Requisitos

- [Rust](https://www.rust-lang.org/tools/install) (con `cargo`)
- Git

## Progreso del libro

| Capítulo | Tema | Práctica | Estado |
|----------|------|----------|--------|
| 1 | Getting Started | `hello-world` | ✅ |
| 2 | Guessing Game | — | ⬜ |
| 3 | Common Concepts | — | ⬜ |
| ... | ... | ... | ... |

Link al libro: https://doc.rust-lang.org/book/title-page.html