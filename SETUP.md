# Setup

This pack is designed for the GitHub profile repository:

`ZZZRRrobots/ZZZRRrobots`

## Files

- `README.md`
- `.github/workflows/contribution-arcade.yml`

## What it does

The workflow generates:

- `github-snake.svg`
- `github-snake-dark.svg`
- `pacman-contribution-graph.svg`
- `pacman-contribution-graph-dark.svg`

The generated files are pushed to an `output` branch and the README displays them directly.

## Important

These are animated SVG visualizations, so they **appear inside the README**. They are not JavaScript games running inside GitHub Markdown.

The Snake project is Platane/snk. The Pac-Man contribution graph project supports Pac-Man, Breakout, Galaga, Puzzle Bobble, Bomberman and Minesweeper. This profile pack intentionally uses only two games: Snake + Pac-Man.

## First run

1. Put the README in the root of your profile repo.
2. Put `contribution-arcade.yml` at `.github/workflows/contribution-arcade.yml`.
3. In the repository, open **Settings → Actions → General**.
4. Make sure workflow permissions allow the workflow to write repository contents.
5. Open **Actions → Update Contribution Arcade → Run workflow**.
6. Wait for it to finish.
7. The `output` branch should appear.
8. Refresh your profile.

If GitHub asks for approval for third-party Actions, approve the workflow/action according to your repository's Actions settings.

## If the generated images do not appear

Check the workflow run first. A failed Action means the SVG files were not generated.

Also verify that the repository is exactly:

`ZZZRRrobots/ZZZRRrobots`

and that the README URLs use the same capitalization/username.

