name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    # Runs at 00:00AM UTC
    - cron: '0 0 * * *'

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master #PLEASE USE MASTER BRANCH
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
          SHOW_PROJECTS: "False"
          SHOW_LINES_OF_CODE: "True"
          SHOW_LOC_CHART: "False"
          LOCALE: "en"

 ### Main skills: 
 ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
 ![SQL](https://img:shields.io/badge/-SQL-001117?style=for-the-badge&logo=sql&labelColor0D1117)&nbsp;
