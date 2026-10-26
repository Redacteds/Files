# Files
File Organizer
# File Organizer

A small Python CLI that sorts the files in a folder into subfolders by type
(Images, Documents, Code, and so on). Supports dry runs and avoids overwriting
existing files.

## Usage

```bash
# Preview changes
python organizer.py ~/Downloads --dry-run

# Organize for real
python organizer.py ~/Downloads
```

## Running tests

```bash
pip install pytest
python -m pytest -q
```

## Features

- Categorizes files by extension (case-insensitive)
- Dry-run mode to preview changes
- Never overwrites: name collisions become `file (1).ext`
- Fully tested with pytest; CI runs on every push via GitHub Actions

## Customizing

Edit the `CATEGORIES` dictionary in `organizer.py` to add your own types.

## License

MIT
