# dirdust-hq

Small Go tool: declutter ~/Downloads in one command

Built for my own use; public in case it helps someone.

## Installation

```bash
go build -o bin/ ./...
```

## Examples

```bash
./bin/dirdust-hq ~/Downloads --dry-run
./bin/dirdust-hq ~/Downloads
```

## Highlights

- Dry-run prints the plan before moving anything
- Skips hidden files and folders by default
- Single static binary, no runtime deps
- Groups files into folders by extension

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
├── go.mod
└── main.go
```

## Development

```bash
go build ./...
go vet ./...
```
