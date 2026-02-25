# Demo Agent

A minimal CLI code-editing agent built in Go, inspired by the Amp note on building an agent.

## What it does

- Runs a terminal chat loop with Claude via the Anthropic Go SDK.
- Maintains conversation history across turns.
- Exposes three tools to the model:
  - `read_file`
  - `list_files`
  - `edit_file`

## Requirements

- Go 1.24+
- `ANTHROPIC_API_KEY` set in your environment

## Run

```bash
go mod tidy
go run main.go
```

## Notes

- This project is intentionally small and straightforward.
- Tool behavior is implemented in `main.go` for clarity.
