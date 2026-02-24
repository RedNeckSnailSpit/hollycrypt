# hollycrypt

A Hollywood-style decryption reveal animation. Because real crypto is boring to watch.

## What is it?

hollycrypt is a visual demo of what a decryption reveal animation could look like in a real application — where data is stored encrypted at rest and only revealed to the owner once they've proven ownership. Instead of data just appearing, it animates from the raw encrypted/hashed value down to the actual plaintext, matrix-style.

Real ciphers don't work this way. Hollywood doesn't care. Neither do we.

**Live demo:** [rednecksnailspit.co.za/hollycrypt_demo](https://rednecksnailspit.co.za/hollycrypt_demo)

## Features

- SHA-256 hash reveal animation with scrambling remaining characters
- Fixed 5-second reveal duration regardless of value length
- Add multiple fields, each animates in sequence
- Fully customisable colours (RGB + Alpha sliders per element)
- Fully customisable font sizes per element
- High-contrast, mobile-friendly customiser panel
- Pure HTML/CSS/JS — no dependencies, no build step

## Usage

Just drop `index.html` somewhere and open it. That's it.

```bash
git clone https://github.com/RedNeckSnailSpit/hollycrypt.git
cd hollycrypt
# Open index.htm in your browser
```

Or serve it:

```bash
npx serve .
# or
php -S localhost:8080
```

## Intended Real-World Use

The animation is designed to represent a flow where:

1. User authenticates and provides a decryption key
2. The encrypted blob is fetched from the DB and displayed as-is — exactly what the DB holds
3. The key decrypts the data client-side and the reveal animation plays
4. The key never touches the DB. The DB never holds plaintext.

hollycrypt is the visual layer for that moment. Plug in your own crypto backend.

## Files

| File | Description |
|------|-------------|
| `index.htm` | The demo itself |
| `README.md` | You're reading it |
| `LICENSE` | Dual license — GPL v3 for non-commercial, commercial license required for for-profit use |

## Attribution

If you use hollycrypt, attribution is required unless you have explicit written permission to omit it:

- **Credit:** RedNeckSnailSpit
- **Link:** [rednecksnailspit.co.za](https://rednecksnailspit.co.za/)

## License

Dual licensed. Free for non-commercial use under GPL v3. Commercial use requires a paid license.

Full licensing information: [legal.rednecksnailspit.co.za](https://legal.rednecksnailspit.co.za)

**TL;DR:** If you're making money from this, we need to talk first.
