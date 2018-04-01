---
layout: default
title: Concentration in Negotiation and Leadership
---

<section class="panel spotlight large left" id="home">
  <div class="content span-5">
    <h1>
      Lead.<br>
      Persuade.<br>
      Collaborate.<br>
    </h1>
  </div>
  <div class="content span-6">
    <h2>The HASS Concentration in Negotiation and Leadership emphasizes an <u>interdisciplinary</u> and <u>hands-on</u> approach to pedagogy in order to provide you with opportunities to reflect on and enhance your <u>decision-making</u>, <u>persuasion</u>, and <u>collaboration</u> capabilities.</h2>
  </div>
  
  <div class="image tinted" data-position="center">
    <img src="images/canyon.jpg" />
  </div>
</section>

<section class="panel color0" id="reqs">
  <div class="inner span-4">
    <h1 class="major">Requirements</h1>
    <p>The requirements consist of two <em>required classes</em> and one <em>elective</em>.</p>
    <h3>Required Classes</h3>
    <table>
      <tr>
        <th>Class</th>
        <th>Name</th>
        <th>Fall</th>
        <th>Spring</th>
      </tr>
      {% for class in site.data.classes %}
      {% if class.group == "required" %}
      <tr>
        <td>{{ class.number }}</td>
        <td>{{ class.name }}</td>
        <td>{{ class.fall }}</td>
        <td>{{ class.spring }}</td>
      </tr>
      {% endif %}
      {% endfor %}  
    </table>
  </div>

  <div class="inner span-4">
    <h3>Electives</h3>
    <table>
      <tr>
        <th>Class</th>
        <th>Name</th>
        <th>Fall</th>
        <th>Spring</th>
      </tr>
      {% for class in site.data.classes %}
      {% if class.group == "electives" %}
      <tr>
        <td>{{ class.number }}</td>
        <td>{{ class.name }}</td>
        <td>{{ class.fall }}</td>
        <td>{{ class.spring }}</td>
      </tr>
      {% endif %}
      {% endfor %}  
    </table>
  </div>
</section>

<section class="panel color1" id="programs">
  <div class="intro span-2">
    <h1 class="major">Programs</h1>
    <p>something</p>
  </div>
  
  <div class="gallery">
    <div class="group span-2">
      {% for program in site.data.programs %}
      <a class="image span-2" href="{{ program.full }}"
         data-position="{{ program.position }}"
         data-name="{{ program.name }}"
         data-url="{{ program.url }}"
         data-description="{{ program.description }}">
        <img src="{{ program.thumbnail }}" />
      </a>
      {% endfor %}
    </div>
  </div>
</section>

<section class="panel color2" id="people">
  <div class="intro span-2">
    <h1 class="major">People</h1>
    <p>something</p>
  </div>
  
  <div class="gallery">
    <div class="group span-2">
      {% for person in site.data.people %}
      <a class="image span-2" href="{{ person.image }}"
         data-position="{{ person.position }}"
         data-name="{{ person.name }}"
         data-url="{{ person.url }}"
         data-description="{{ person.description }}">
        <img src="{{ person.image }}" />
      </a>
      {% endfor %}
    </div>
  </div>
</section>

