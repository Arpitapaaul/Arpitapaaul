python3 << 'EOF'
with open('/mnt/user-data/outputs/README.md', 'r') as f:
    content = f.read()

old_stats = '''<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Arpitapaaul&show_icons=true&theme=radical&hide_border=true&count_private=true" height="170"/>
&nbsp;&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Arpitapaaul&layout=compact&theme=radical&hide_border=true" height="170"/>

<br/><br/>

<img src="https://streak-stats.demolab.com?user=Arpitapaaul&theme=radical&hide_border=true&border_radius=10&date_format=j%20M%5B%20Y%5D" width="65%"/>

</div>'''

new_stats = '''<div align="center">

### 📊 Stats & 🔥 Streak

<img src="https://github-readme-stats.vercel.app/api?username=Arpitapaaul&show_icons=true&theme=radical&hide_border=true&count_private=true&bg_color=0d0d0d&title_color=ff6eb4&icon_color=ff6eb4&text_color=ffffff&border_radius=10" width="48%"/>
&nbsp;
<img src="https://streak-stats.demolab.com?user=Arpitapaaul&theme=radical&hide_border=true&border_radius=10&background=0d0d0d&stroke=ff6eb4&ring=ff6eb4&fire=ff6eb4&currStreakLabel=ff6eb4&sideLabels=ff6eb4&dates=888888" width="48%"/>

</div>

---

<div align="center">

### 📈 Contribution Graph

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Arpitapaaul&bg_color=0d0d0d&color=c084fc&line=ff6eb4&point=ffffff&area=true&area_color=c084fc&hide_border=true&radius=10" width="95%"/>

</div>

---

<div align="center">

### 💻 Most Used Languages

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Arpitapaaul&layout=donut&theme=radical&hide_border=true&bg_color=0d0d0d&title_color=ff6eb4&text_color=ffffff&border_radius=10" width="40%"/>

</div>'''

content = content.replace(old_stats, new_stats)

with open('/mnt/user-data/outputs/README.md', 'w') as f:
    f.write(content)

print("Done!" if 'activity-graph' in content else "Not replaced!")
EOF
Output
