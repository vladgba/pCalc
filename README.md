# pCalc

A small Android calculator where your own formulas are keys. Type `bmi(kg, m) = kg ÷ m^2` once and it sits next to the digits from then on, together with a function plotter and a pull-down history.

## Features

- **Your formulas as keys.** Define functions and constants, call them like built-ins, reorder, edit or delete them. Long-press a formula key to edit it. Formulas can call each other, recursion included.
- **Three keypad pages.** Swipe between **My formulas**, the **123** numpad and **Functions**. Inserting a formula or function jumps back to the numpad.
- **Live result.** The answer is previewed while you type. Tap anywhere in the expression to move the cursor; the system keyboard never opens.
- **Textbook display.** `2^10` is shown as 2¹⁰, and towers like `2^3^2` stack.
- **Graphs.** Plot several `y = f(x)` curves at once: drag to pan, pinch to zoom, tap to trace. Pressing `=` on an expression with `x` opens the graph.
- **History.** Pull down on the display. Tap an entry to insert its result, long-press to restore its expression.
- **DEG / RAD** toggle, light and dark theme.
- **No ads, no network, no data collection.**

## Permissions

pCalc requests no permissions.

### Notes

- The formula syntax, the full list of functions and operator precedence are in the [guide](docs/GUIDE.md#writing-formulas).
- Graphs always use radians, whatever the DEG / RAD setting.

## Build

Requires Android 8.0+ (API 26). Built with Kotlin on the plain Android framework, without libraries.

```bash
./gradlew assembleRelease
```

The APK is written to `app/build/outputs/apk/release/`.

## License

See [LICENSE](LICENSE).
