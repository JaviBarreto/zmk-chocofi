
# ZMK Config - Chocofi Layout Optimizado

Este repositorio contiene la configuración personalizada para tu teclado **Chocofi** usando ZMK, con compilación automática vía **GitHub Actions** y publicación de firmware `.uf2` en cada push.

---

## 🔧 Estructura del Repositorio

```
.
├── config/
│   └── chocofi/
│       ├── keymap.dtsi        # Distribución principal Dvorak
│       ├── combos.dtsi        # Combos inteligentes (F+J → Esc, etc.)
│       ├── tap_dances.dtsi    # Tap Dances extendidos: ;, :, =>, ->, etc.
│       └── macros.dtsi        # Comandos como git commit, npm run dev, etc.
├── .github/
│   └── workflows/
│       └── build.yml          # Flujo GitHub Actions + release automático
└── west.yml                   # Archivo de manifest de ZMK
```

---

## ⌨️ Capas de Teclado

| Capa  | Nombre           | Función principal                                                  |
|-------|------------------|--------------------------------------------------------------------|
| 0     | Base             | Dvorak modificado con Home Row Mods y Tap Dance extendido         |
| 1     | Navegación       | Flechas, Home/End, PgUp/PgDn, Ctrl+Z/S/C/V/F                      |
| 2     | Símbolos         | {}, [], (), <>, =, +, *, /, |, ;, :, etc.                         |
| 3     | Funciones        | F1–F12, volumen, media, reset, bluetooth toggle                   |
| 4     | Numérica         | 0–9, punto, coma, +, -, *, /                                      |
| 5     | Macros IDE/CLI   | git commit -m "", npm run dev, artisan migrate, VS Code commands  |

---

## 🚀 Cómo Usarlo

1. **Sube todo el contenido de este repositorio a GitHub**
2. Realiza un `git push`
3. Ve a la pestaña **Actions** en GitHub
4. Al terminar la compilación, visita la pestaña **Releases**
5. Descarga los archivos `.uf2` generados y flashea en tu teclado

---

## 🖱 ¿Agregar capa de mouse?

Sí, es **altamente recomendable** si:

- Usas un teclado sin mouse externo frecuentemente
- Quieres moverte en el sistema sin soltar el teclado

Podría incluir:
- IJKL para mover el cursor
- U/N para scroll up/down
- H para click izquierdo, ; para derecho

¿Quieres que la agregue como capa 6?
