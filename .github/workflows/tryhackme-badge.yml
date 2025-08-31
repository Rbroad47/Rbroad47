name: Update TryHackMe badge

on:
  schedule:
    - cron: "0 12 * * *"   # runs daily at 12:00 UTC
  workflow_dispatch:        # allow manual runs

permissions:
  contents: write           # allow the workflow to commit the updated image

jobs:
  update-badge:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: p4p1/tryhackme-badge-workflow@v1
        with:
          username: rbroad
          image_path: assets/thm_propic.png
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
