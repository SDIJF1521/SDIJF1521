### Hi there 👋

<!--
**SDIJF1521/SDIJF1521** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

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
<div align="center"> <img height="137px" src="https://github-readme-stats.vercel.app/api?username=SDIJF1521&hide_title=true&hide_border=true&show_icons=trueline_height=21&text_color=000&icon_color=000&bg_color=0,ea6161,ffc64d,fffc4d,52fa5a&theme=graywhite" /> </div>
# Visit https://github.com/lowlighter/metrics#-documentation for full reference
name: Metrics
on:
  # Schedule updates (each hour)
  schedule: [{cron: "0 * * * *"}]
  # Lines below let you run workflow manually and on each commit
  workflow_dispatch:
  push: {branches: ["master", "main"]}
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Your GitHub token
          # The following scopes are required:
          #  - public_access (default scope)
          #  - repo
          # The following additional scopes may be required:
          #  - read:org      (for organization related metrics)
          #  - read:user     (for user related data)
          #  - read:packages (for some packages related data)
          #  - repo          (optional, if you want to include private repositories)
          token: ${{ secrets.METRICS_TOKEN }}

          # Options
          user: SDIJF1521
          template: classic
          base: header, activity, community, repositories, metadata
          config_timezone: Asia/Shanghai
          plugin_calendar: yes
          plugin_calendar_limit: 1
          plugin_code: yes
          plugin_code_days: 5
          plugin_code_lines: 12
          plugin_code_load: 300
          plugin_code_skipped: https://github.com/SDIJF1521/qqai/blob/main/QQAI/qqai/plugins/%E4%B8%8D%E8%89%AF%E8%AF%AD%E5%8F%A5%E6%92%A4%E5%9B%9E.py
          plugin_code_visibility: all
          plugin_habits: yes
          plugin_habits_charts_type: classic
          plugin_habits_days: 14
          plugin_habits_facts: yes
          plugin_habits_from: 200
          plugin_habits_languages_limit: 8
          plugin_habits_languages_threshold: 0%
          plugin_isocalendar: yes
          plugin_isocalendar_duration: full-year
          plugin_languages: yes
          plugin_languages_analysis_timeout: 15
          plugin_languages_analysis_timeout_repositories: 7.5
          plugin_languages_categories: markup, programming
          plugin_languages_colors: github
          plugin_languages_limit: 8
          plugin_languages_recent_categories: markup, programming
          plugin_languages_recent_days: 14
          plugin_languages_recent_load: 300
          plugin_languages_sections: most-used
          plugin_languages_threshold: 0%
          plugin_nightscout: yes
          plugin_nightscout_datapoints: 12
          plugin_nightscout_highalert: 180
          plugin_nightscout_lowalert: 80
          plugin_nightscout_urgenthighalert: 250
          plugin_nightscout_urgentlowalert: 50
          plugin_nightscout_url: https://example.herokuapp.com
          plugin_support: yes
          plugin_traffic: yes
          plugin_wakatime: yes
          plugin_wakatime_days: 7
          plugin_wakatime_limit: 5
          plugin_wakatime_repositories_visibility: all
          plugin_wakatime_sections: time, projects, projects-graphs, languages, languages-graphs, editors, os
          plugin_wakatime_url: https://wakatime.com
          plugin_wakatime_user: current
<div align="center"> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SDIJF1521&hide_title=true&hide_border=true&layout=compact&langs_count=6&text_color=000&icon_color=fff&bg_color=0,52fa5a,4dfcff,c64dff&theme=graywhite" /> </div>
