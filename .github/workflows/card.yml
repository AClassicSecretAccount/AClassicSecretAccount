name: Update Minecraft Contribution Card

on:
  schedule:
    # Run once every hour
    - cron: '0 * * * *'
  workflow_dispatch: # Allows manual trigger from Actions tab
  push:
    branches:
      - main
    paths-ignore:
      - 'README.md'

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Generate Minecraft Profile Card
        uses: mertcetn/minecraft-github-profile@main
        # Zero configuration! Built-in token is used automatically.
