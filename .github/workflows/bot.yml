name: bot
on: workflow_dispatch
jobs:
  run:
    runs-on: ubuntu-latest
    timeout-minutes: 360
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: "3.11"
      - run: python NetSTRIK_bot.py
        env:
          BOT_TOKEN: ${{ secrets.BOT_TOKEN }}
