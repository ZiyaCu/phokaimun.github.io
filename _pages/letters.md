---
title: "Letters"
permalink: /letters/
layout: splash
header:
  overlay_image: /assets/images/background.jpg
  overlay_color: "#000"
  overlay_filter: "0.4"

persons:
  - name: "Ege Kağan Güncan"
    title: "Secretary General"
    image_path: /assets/images/press.jpeg
    letter_html: |
      <p>Dear Delegates, Organizing Team, and Academic Team Candidates,</p>
      <p>It is my great pleasure and honor to extend to you a warm greeting to the First Annual Session of the Çağlı Model United Nations.</p>
      <p>As Secretary General, I am delighted to welcome each of you to what promises to be an inspiring and enriching experience...</p>
      <p>Whether you are applying as a delegate, an academic team member, or part of the organization, your role will be instrumental in shaping the success and spirit of CMUN. I look forward to witnessing your passion, ideas, and leadership as we come together to tackle global challenges through dialogue and diplomacy.</p>
      <p>Join us in making history at our inaugural session, where every voice matters and every perspective counts.</p>
      <p>Yours sincerely,<br><strong>Ege Kağan Güncan</strong><br><em>Secretary General</em></p>

  - name: "Duru Söylemezoğlu"
    title: "Director General"
    image_path: /assets/images/press.jpeg
    letter_html: |
      <p>Hello everyone,</p>
      <p>My name is Duru Söylemezoğlu. As a member of the executive team of the First Official Session of Çağlı Model United Nations, I would like to express how pleased I am to welcome you all in advance. I hope to see everyone at this conference, which will take shape with your valuable participation and support.</p>
      <p>Our executive team, composed of students from various schools, shares a common goal: to organize a conference in Çağlı and to make it accessible to a wide student audience.</p>
      <p>What distinguishes this conference from previous ones is the effort and care put into every step of the preparation process. With a strong sense of responsibility and a well-structured task distribution, our main goal is to ensure that participants feel satisfied and happy in every aspect of the event.</p>
      <p>Yours sincerely,<br><strong>Duru Söylemezoğlu</strong><br><em>Director General</em></p>
---

<div class="letter-container">
  {% for person in page.persons %}
    <div class="letter-column">
      <div class="letter-header">
        <img src="{{ person.image_path | relative_url }}" alt="{{ person.name }}" class="profile-image">
        <div class="person-details">
          <h3 class="person-name">{{ person.name }}</h3>
          <p class="person-title">{{ person.title }}</p>
        </div>
      </div>
      <div class="letter-body">
        {{ person.letter_html | markdownify }}
      </div>
    </div>
  {% endfor %}
</div>
