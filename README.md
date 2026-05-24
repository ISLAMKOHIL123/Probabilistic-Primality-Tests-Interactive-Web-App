# Probabilistic Primality Tests – Interactive Web App

Implementation and comparative analysis of three probabilistic primality tests:
Fermat, Solovay–Strassen, and Miller–Rabin. Built as a single-file web app with
real-time performance visualization.

🔗 **Live demo**: https://tparmo1.vercel.app

## What it does

- Tests arbitrarily large numbers for primality using JavaScript `BigInt`
- Runs all three tests simultaneously and compares results
- Displays execution times with a real-time Chart.js bar chart
- Shows error probability for each test and iteration count

## Algorithms Implemented

| Test | Error Bound | Detects Carmichael | Used in Practice |
|------|-------------|-------------------|-----------------|
| Fermat | ≤ 2⁻ᵏ | No | Rarely |
| Solovay–Strassen | ≤ 2⁻ᵏ | Yes | Rarely |
| Miller–Rabin | ≤ 4⁻ᵏ | Yes | **Standard** |

## Key Findings

- Miller–Rabin is 30–50% faster than Solovay–Strassen
- At k=20 iterations, Miller–Rabin error probability < 9.1×10⁻¹³
- Miller–Rabin is deterministic for n < 2⁶⁴ with fixed bases

## Tech Stack

Pure HTML5 + CSS3 + JavaScript ES6+ — no build step, no dependencies to install.
Uses Bootstrap 5 and Chart.js via CDN.

## Usage

```bash
# Just open the file
open index.html
```

Or visit the live demo directly.

## Author

KOHIL Islam – USTHB, Cryptographie / Algèbre, 2025–2026
