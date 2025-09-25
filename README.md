## Hi there 👋
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=435&lines=Welcome+come+to+my+Github.)](https://git.io/typing-svg)
name: fornever
on:
  push:
    branches:
      - master
  pull_request:
    branches:
      - master
jobs:
  coverage:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: ArtiomTr/jest-coverage-report-action@v2
      - name: Upload coverage reports to Codecov
        uses: codecov/codecov-action@v5
        env:
          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
<!--
**fornever-lw/fornever-lw** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
