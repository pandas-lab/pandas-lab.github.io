---
layout: page
title: About PANDAS Lab
subtitle: "Politics × (AI + Data Science)<br>University of North Carolina at Charlotte"
featured-img: red-panda-01.jpeg
permalink: /about/
---

# PANDAS Lab

The Politics, AI, and Data Science Lab (PANDAS) is a research lab that applies machine learning and statistical techniques to the study of politics, especially in areas of conflict, propaganda, misinformation, and cybersecurity. PANDAS is housed within UNC Charlotte's Department of Political Science and Public Administration. We work with students from across the University and beyond. Learn how to [join our team](/join.html).

# Current Research Projects

* Forecasting political conflict at the micro level
* Measuring populist rhetoric in text and speech
* Coding multidimensional concepts with language models
* Measuring shifts in territorial control during wars
* Government-sponsored information manipulation
* Data collection and inference on cyberconflict actors

# Our Team
<a href="#team"></a>

<div class="post-list" style="justify-content: center" itemscope="" itemtype="http://schema.org/Blog">
            {% for author in site.authors %}
            {% if author.role == "PI" %}
            <div class="author-card">
              <center>
              <div style="min-width:250px; min-height:250px; max-width:250px; max-height:250px; border-radius:50%; overflow:hidden; background-color:black">
                <img src="{{ author.headshot }}" style="width:100%; margin:0; padding:0">
              </div><br>
               <h3>{{ author.name }}</h3>
               {{ author.title }}, {{ author.institution }} <br>
                {% if author.homepage %}
                  <a href="{{ author.homepage }}" class="label onwhite">Homepage</a> <a href="{{ author.github }}" class="label onwhite">Github</a> <br>
                {% endif %}
              </center>
            </div>
            {% endif %}
            {% endfor %}
            {% for author in site.authors %}
            {% if author.role == "Current" %}
            <div class="author-card">
              <center>
              <div style="min-width:250px; min-height:250px; max-width:250px; max-height:250px; border-radius:50%; overflow:hidden; background-color:black">
              	{% if author.headshot %}
                	<img src="{{ author.headshot }}" style="width:100%; margin:0; padding:0">
                {% else %}
                	<img src="/assets/img/panda-headshot.jpeg" style="width:100%; margin:0; padding:0">
                {% endif %}
              </div><br>
               <h3>{{ author.name }}</h3>
               {{ author.title }}, {{ author.institution }} <br>
                {% if author.homepage %}
                  <a href="{{ author.homepage }}" class="label onwhite">Homepage</a> 
                {% endif %}
                {% if author.github %}
                  <a href="{{ author.github }}" class="label onwhite">Github</a> <br>
                {% endif %}
              </center>
            </div>
            {% endif %}
            {% endfor %}
</div>

## Former Members
<!-- <div class="callout"> -->
<ul>
{% for author in site.authors %}
    {% if author.role == "Former" %}
        <li> {{ author.name }} </li>
    {% endif %}
{% endfor %}
</ul>
<!-- </div> -->


# Contribute
<iframe id='kofiframe' src='https://ko-fi.com/pandaslab/?hidefeed=true&widget=true&embed=true&preview=true' style='border:none;width:100%;padding:4px;background:#f9f9f9;' height='712' title='pandaslab'></iframe>


# Acknowledgements  

This website is compiled with [Jekyll](https://jekyllrb.com/) using a modified version of the [Sleek theme](https://github.com/janczizikow/sleek). Some of our images are produced with [Stable Diffusion XL](https://huggingface.co/papers/2307.01952). We use 
[Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) by AUTOMATIC1111 and [Vintage Anime LoRA](https://civitai.com/models/313318/vintage-anime).