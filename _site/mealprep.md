---
title: Meal Prep
layout: page

---


<!-- INTRO -->
<div class="n_about_intro">
<div id="n_titles"><h2>ReLeaf Meal Prep</h2>
</div>
</div>
<div class="mealprep">
{% for recipe in mealprep %}
<div class="recipeinformation"> 

<img src="{{recipe.src}}" class="c50;">
<div class="mealprepdeets">
<h6>{{recipe.day}}</h6>
<h2>{{recipe.name}}<h2>
<p>{{recipe.description}} </p>
<h5>{{recipe.time}}</h5>
<h5>{{recipe.ingredients}}</h5>
<h5>{{recipe.calories}}</h5>
<button class="hero-button"><a href="/mealprep/{{ recipe.day | slug }}">Learn More</a> </button>
</div>
</div>
    {% endfor %}
</div>
