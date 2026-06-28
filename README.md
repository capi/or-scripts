# or-scripts

CLI tools for media generation via [OpenRouter](https://openrouter.ai/).

- **orimg** — Image generation (Gemini, FLUX, Recraft)
- **orsong** — Music generation (Lyria Pro / Lyria Clip)

## Usage

```bash
orimg "prompt" -o output.png -m google/gemini-2.5-flash-image -r 16:9
orsong "prompt" -o output.mp3
```

## Auth

Requires `OPENROUTER_API_KEY` env var or `~/.config/openrouter/api_key`.

## Models

| Tool | Default Model | Cost |
|------|--------------|------|
| orimg | `google/gemini-2.5-flash-image` | ~$0.04 |
| orsong | `google/lyria-3-pro-preview` | $0.08/song |
| orsong --clip | `google/lyria-3-clip-preview` | $0.04/clip |
