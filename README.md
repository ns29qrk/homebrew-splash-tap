# Splash Homebrew Tap (mise-compatible fork)

Forked from [incoai/homebrew-tap](https://github.com/incoai/homebrew-tap) to support installation via [mise](https://mise.jdx.dev).

## Install via mise (Recommended)

### 1. Add the Tap
```sh
mise bootstrap packages brew tap ns29qrk/splash-tap https://github.com/ns29qrk/homebrew-splash-tap.git
```

### 2. Install Splash
```sh
mise bootstrap packages use -g brew:ns29qrk/splash-tap/splash
```

### Using in `mise.toml`
```toml
[bootstrap.brew.taps]
"ns29qrk/splash-tap" = "https://github.com/ns29qrk/homebrew-splash-tap.git"

[bootstrap.packages]
"brew:ns29qrk/splash-tap/splash" = "latest"
```

Apply the configuration:
```sh
mise bootstrap packages apply --manager brew
```

---

## Install via Homebrew

```sh
brew install ns29qrk/splash-tap/splash
```

---

## Formulae

| Formula | What it is | Requirements |
| --- | --- | --- |
| `splash` | Local inference engine for Apple silicon, built around the model. [Repository](https://github.com/incoai/splash) · [Launch post](https://inco.ai/blog/splash/) | M3 or newer Mac, macOS 26.4 or later, 36 GB of unified memory |

Report problems with `splash` in its [official repository](https://github.com/incoai/splash).
