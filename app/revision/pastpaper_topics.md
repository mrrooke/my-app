---
layout: post
title: Past Paper Questions by Topics
list: true
archive:
  - file_path: /revision/pastpaper_topics/a_star1h.pdf
    title: A* Paper 1
    strand: A*
  - file_path: /revision/pastpaper_topics/a_star2h.pdf
    title: A* Paper 2
    strand: A*
  - file_path: /revision/pastpaper_topics/algebra.pdf
    title: Algebra
    strand: Algebra
  - file_path: /revision/pastpaper_topics/bounds.pdf
    title: Bounds
    strand: Number
  - file_path: /revision/pastpaper_topics/boxplots.pdf
    title: Box Plots
    strand: Data
  - file_path: /revision/pastpaper_topics/Circle Theorems.pdf
    title: Circle Theorems
    strand: Shape
  - file_path: /revision/pastpaper_topics/cumfreq.pdf
    title: Cumulative Frequency Curves
    strand: Data
  - file_path: /revision/pastpaper_topics/fractions.pdf
    title: Fractions
    strand: Number
  - file_path: /revision/pastpaper_topics/frequency.pdf
    title: Frequency Tables
    strand: Data
  - file_path: /revision/pastpaper_topics/histograms2.pdf
    title: Histograms
    strand: Data
  - file_path: /revision/pastpaper_topics/locus.cons.pdf
    title: Loci and Constructions
    strand: Shape
  - file_path: /revision/pastpaper_topics/number1.pdf
    title: Number
    strand: Number
  - file_path: /revision/pastpaper_topics/Percentages.pdf
    title: Percentages
    strand: Number
  - file_path: /revision/pastpaper_topics/Probability Tree.pdf
    title: Probability Trees
    strand: Data
  - file_path: /revision/pastpaper_topics/pythagoras.pdf
    title: Pythagoras
    strand: Shape
  - file_path: /revision/pastpaper_topics/quad.graphs.pdf
    title: Quadratic Graphs
    strand: Algebra
  - file_path: /revision/pastpaper_topics/questionnaire (1).pdf
    title: Questionnaires
    strand: Data
  - file_path: /revision/pastpaper_topics/scattergraphs.pdf
    title: Scatter Graphs
    strand: Data
  - file_path: /revision/pastpaper_topics/sequences.pdf
    title: Sequences
    strand: Algebra
  - file_path: /revision/pastpaper_topics/simultaneous.pdf
    title: Simultaneous Equations
    strand: Algebra
  - file_path: /revision/pastpaper_topics/surds.pdf
    title: Surds
    strand: Number
  - file_path: /revision/pastpaper_topics/Transformations & Symmetry.pdf
    title: Transformations and Symmetry
    strand: Shape
  - file_path: /revision/pastpaper_topics/trial.pdf
    title: Trial and Improvement
    strand: Algebra
  - file_path: /revision/pastpaper_topics/trigonometry.pdf
    title: Trigonometry
    strand: Shape
  - file_path: /revision/pastpaper_topics/vectors.pdf
    title: Vectors
    strand: Shape
---

If you are revising purely from past papers, it usually means moving from one
topic to another and not covering any of them in any great detail. The booklets
below contain most of the question types that have been asked in the last ten
years. This means that they are great for focused revision. The A* booklets
contain topics that come up less often, but could make the difference between
you achieving the grade you want.

**Caution:** These booklets will only provide you with exam style practice
questions. They **will** not teach you a concept, or give you the easier
questions that are needed to build fluency. If you do not know a topic, I would
recommend looking at [HegartyMaths](www.hegartymaths.net) or
[MathsWatch](www.mathswatchvle.com) to develop your understanding first.sh

I will try and gradually upload answers to these booklets, so check back if you
need to mark the work that you have completed.

## A*
<table class="table">
<tbody>
{% assign posts = page.archive| where: "strand", "A*" %}
{% for post in posts %}
    {% assign loopindex = forloop.index | modulo:2 %}  
    {% if loopindex == 1 %}
    <tr>
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    {% else %}
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    </tr>
    {% endif %}
{% endfor %}
</tr>
</tbody>
</table>


## Number
<table class="table">
<tbody>
{% assign posts = page.archive| where: "strand", "Number" %}
{% for post in posts %}
    {% assign loopindex = forloop.index | modulo:2 %}  
    {% if loopindex == 1 %}
    <tr>
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    {% else %}
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    </tr>
    {% endif %}
{% endfor %}
</tr>
</tbody>
</table>

### Algebra
<table class="table">
<thead></thead>
<tbody>
{% assign posts = page.archive| where: "strand", "Algebra" %}
{% for post in posts %}
    {% assign loopindex = forloop.index | modulo:2 %}  
    {% if loopindex == 1 %}
    <tr>
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    {% else %}
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    </tr>
    {% endif %}
{% endfor %}
</tr>
</tbody>
</table>

### Shape
<table class="table">
<tbody>
{% assign posts = page.archive| where: "strand", "Shape" %}
{% for post in posts %}
    {% assign loopindex = forloop.index | modulo:2 %}  
    {% if loopindex == 1 %}
    <tr>
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    {% else %}
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    </tr>
    {% endif %}
{% endfor %}
</tbody>
</table>

### Data
<table class="table">
<tbody>
{% assign posts = page.archive| where: "strand", "Data" %}
{% for post in posts %}
    {% assign loopindex = forloop.index | modulo:2 %}  
    {% if loopindex == 1 %}
    <tr>
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    {% else %}
    <td class="col-md-3">
        <a href="{{ post.file_path }}">{{ post.title }}</a>
    </td>
    </tr>
    {% endif %}
{% endfor %}
</tr>
</tbody>
</table>
