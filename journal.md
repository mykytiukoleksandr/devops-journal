- 2026-10-11: set up Git, Python, Ubuntu (WSL)
- 2026-10-12: practiced Linux commands (mkdir -p, touch, nano, head, tail, wc, cp -r, mv)
- 2026-10-13: learned sudo, chown, chmod.
- 2026-10-13 Learned how to use find and grep using pipe

## 2026-10-16 - Day 5: processes, resources, packages, services

**Done**
- Processes: `ps aux`, `jobs`, `kill`, background jobs with `&`, sorting by memory.
- Resources and packages: `df -h`, `free -h`, `du -sh`, `apt update/install`.
- Services: installed nginx, `systemctl status/start/stop/enable/disable`, `journalctl -u`.
- Project `server-health`: bash script that writes a system report, README, `.gitignore`, 4 commits on GitHub.

**What went wrong**
- `--sort=%mem` instead of `--sort=-%mem` (minus = heaviest first).
- `systemctl` changes need `sudo`; reading status does not.
- `date && hostname >> file` redirected only `hostname`; each command needs its own `>>`.
- `.gitignore` was created in `scripts/` instead of the repo root.
- Script did not run: no execute permission, fixed with `chmod +x`.
- README mentioned `report.sh`, but the file is `health.sh`.

**Cards to repeat tomorrow**
- `du -sh` for folder size
- `sudo` for state-changing systemctl commands
- `journalctl -u nginx -n 10 --no-pager`

**Carry over**
- Bonus: report file name with the date and a WARNING if nginx is stopped (needs `if`).
