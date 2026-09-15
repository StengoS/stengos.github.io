---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I'm a 4th-year software engineering Ph.D. student at University of California, Irvine (UCI)'s [Informatics Department](https://www.informatics.uci.edu/). I am advised by [Dr. Joshua Garcia](https://jgarcia.ics.uci.edu/). 

<br>

## Research Interests

<div class="interest-grid">

  <div class="interest-card">
    <div class="interest-card__icon"><i class="fa-solid fa-chalkboard-user" aria-hidden="true"></i></div>
    <p class="interest-card__title">CS Education</p>
    <p class="interest-card__desc">Student-run cybersecurity clubs, upcycled cyber ranges</p>
  </div>

  <div class="interest-card">
    <div class="interest-card__icon"><i class="fa-solid fa-shield-halved" aria-hidden="true"></i></div>
    <p class="interest-card__title">Software Security</p>
    <p class="interest-card__desc">Bug bounties, CVEs, and open-source maintainers</p>
  </div>

  <div class="interest-card">
    <div class="interest-card__icon"><i class="fa-solid fa-robot" aria-hidden="true"></i></div>
    <p class="interest-card__title">AI &amp; Security</p>
    <p class="interest-card__desc">AI red teaming, AI security education</p>
  </div>

</div>

<br>

## Recent Highlights

<ul class="timeline">
  <li class="timeline__item">
    <span class="timeline__date">Sep. 14, 2026</span>
    <p class="timeline__title">Netsiege: A Long-Form, Club-Led King-of-the-Hill Competition for Accessible Cybersecurity Training</p>
    <p class="timeline__desc">Paper accepted to SIGCSE 2027 (~25.8% acceptance rate).</p>
    <p class="timeline__meta">ACM Technical Symposium on Computer Science Education (SIGCSE) 2027</p>
  </li>
  <li class="timeline__item">
    <span class="timeline__date">Aug. 7, 2026</span>
    <p class="timeline__title"><a href="https://info.defcon.org/defcon34/content/68125">Student-Run Cyber Clubs - Why They Matter &amp; Digital Playgrounds</a></p>
    <p class="timeline__desc">Gave a presentation on cyber clubs at DEFCON 34 to the .EDU Community.</p>
    <p class="timeline__meta">DEFCON 34</p>
  </li>
  <li class="timeline__item">
    <span class="timeline__date">May 19, 2025</span>
    <p class="timeline__title"><a href="https://news.uci.edu/2025/05/19/uc-irvine-team-wins-national-collegiate-cyber-defense-competition/">UC Irvine team wins National Collegiate Cyber Defense Competition</a></p>
    <p class="timeline__desc">Competed as the corporate lead of Cyber@UCI's CCDC team, where we won 1st at Nationals!</p>
    <p class="timeline__meta">UC Irvine News</p>
  </li>
  <li class="timeline__item">
    <span class="timeline__date">Mar. 19, 2025</span>
    <p class="timeline__title"><a href="https://www.oit.uci.edu/2025/03/19/cybersecurity-zotgpt-collab/">Securing the Future: ZotGPT and Cyber@UCI Unite to Fortify Generative AI Defenses</a></p>
    <p class="timeline__desc">Set up and facilitated this collaboration, managing the student team and keeping UCI OIT updated throughout.</p>
    <p class="timeline__meta">UCI Office of Data and Information Technology</p>
  </li>
  <li class="timeline__item">
    <span class="timeline__date">Jan. 28, 2025</span>
    <p class="timeline__title"><a href="https://ics.uci.edu/2025/01/28/uc-irvines-codesafe-platform-wins-50000-in-global-edtech-competition/">UC Irvine's Codesafe Platform Wins $50,000 in Global EdTech Competition</a></p>
    <p class="timeline__desc">Led development of Codesafe as first author, winning the DARPA + Tools Catalyst Award.</p>
    <p class="timeline__meta">UCI Donald Bren School of Information &amp; Computer Sciences</p>
  </li>
  <li class="timeline__item">
    <span class="timeline__date">Jul. 1, 2024</span>
    <p class="timeline__title"><a href="https://news.uci.edu/2024/07/01/cyberuci-team-places-fourth-in-national-cybersecurity-competition/">Cyber@UCI team places fourth in national cybersecurity competition</a></p>
    <p class="timeline__desc">Competed as a member of Cyber@UCI's CCDC team at National CCDC Nationals.</p>
    <p class="timeline__meta">UC Irvine News</p>
  </li>
</ul>

<br>

## Selected Publications

<ul class="pub-list">
{% for post in site.publications reversed limit:3 %}
  {% if post.id %}
    {% assign pub_title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
  {% else %}
    {% assign pub_title = post.title %}
  {% endif %}
  <li class="pub-list__item">
    <p class="pub-list__title"><a href="{{ post.link | default: post.url }}">{{ pub_title }}</a></p>
    {% if post.forthcoming %}
    <p class="pub-list__meta">To appear in <i>{{ post.venue }}</i>{% if post.acceptance_rate %}, ~{{ post.acceptance_rate }} acceptance rate{% endif %}</p>
    {% else %}
    <p class="pub-list__meta">Published in <i>{{ post.venue }}</i>{% if post.acceptance_rate %}, ~{{ post.acceptance_rate }} acceptance rate{% else %}, {{ post.date | default: "1900-01-01" | date: "%Y" }}{% endif %}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>

*See all [publications](/publications/).*

<br>

I may not always be available for collaboration, but please don't hesitate to reach out if any of my work is of interest or if you would just like to work together. Please also feel free to reach out if you have any questions or just want to chat!



*If you'd like more up-to-date information on my profile, please contact [skngo1@uci.edu](mailto:skngo1@uci.edu).*
