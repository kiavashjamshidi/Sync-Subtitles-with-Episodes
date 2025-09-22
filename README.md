# subtitle-syncer

A tiny CLI to batch-align `.srt` subtitles with TV-show episodes. Supports global time shift (± ms/sec), per-file matching, and dry-run checks.

## Features
- Batch sync subtitles to episodes
- Global offset (positive/negative)
- Simple filename matching (S01E02 style)
- Dry run & backup original files

## Usage
python subtitle_sync.py \
  --subs ./subs/ \
  --videos ./episodes/ \
  --offset +2.5s \
  --backup

## Args
--subs      Path to folder with .srt files
--videos    Path to folder with episode files
--offset    Time shift (e.g., +2.5s, -1200ms)
--dry-run   Show changes without writing
--backup    Save original .srt alongside

## Notes
Tested on Python 3.10+. Works on macOS/Linux/Windows.
