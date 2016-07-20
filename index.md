---
layout: index
title: Home
comments: false
description: "Hello everybody. This is about Manikanta, an Amateur Astronomer and an easy going comp. science undergrad at Indian Institute of Technology, Kanpur. He isn't much but, yeah, here you go"
---

<center>
	<h2>Hi!</h2>
</center>
Hello everybody. This is about Manikanta, an Amateur Astronomer and an easy going comp. science undergrad at Indian Institute of Technology, Kanpur. He isn't much but, yeah, here you go

<hr class="hr-line">

<center>
	<h2>What interests me?</h2>
</center>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/ml.png">
        </div>
    <h3 class="centered">Machine Learning</h3>
        <p>This is my primary field of interest. I have this weird fetish for finding patterns in any data, must be my OCD! I'm currently working on course project regarding the analysis of surveliience footage.</p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/eye.png">
        </div>
        <h3 class="centered">Computer Vision</h3>
        <p>Image processing and computer vision are interesting topics! I worked on gesture recognition with simple background subtraction techniques.</p>
    </div>
</div>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/universe.png">
        </div>
        <h3 class="centered">Astro Physics</h3>
        <p>I like the dark skies a lot. I spend many nights, just lying there and watch them stars twinkle. I also like cosmology, stellar tatistics and studying the large-scale structure of the universe. Did I mention I was in the Astronomy OCSC Camp - 2013?</p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/music.png">
        </div>
        <h3 class="centered">Music</h3>
        <p>I have got a really wanky taste in music, mostly electronic pop. Music washes away from the soul the dust of everyday life. What's better than to plug in my earphones and dream with volume on full. Stalk on my last.fm to see for yourselves.</p>
    </div>
</div>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/food.png">
        </div>
        <H3 class="centered">Food</H3>
        <p>
            I can cook too. When I've nothing else to do, you can always find me in the kitchen cooking delicous food and eating it. If I ever invite you over, trust me, it'll be fireworks in your mouth.
        </p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/earth.png">
        </div>
        <h3 class="centered">Everthing Else</h3>
        <p>Besides all of that, I like to cycle and walk randomly and bump into people. I also trek mountains sometimes and like to go places </p>
    </div>
</div>


<hr class="hr-line">

<center>
	<h2>Recent Posts</h2>
</center>

<div class="post-list">
    {% for post in site.posts offset: 0 limit: 4 %}
        {% cycle 'add row' : '<div class="row">', nil %}
            <div class="col-md-6">
                <div class="image">
                    <img src="{{ site.url }}/assets/img/placeholder-big.jpg" alt="" />
                    <div class="caption">
                        <h3>{{ post.title }}</h3>
                        <p>{{ post.excerpt }}</p>
                        <a href="{{ site.url }}{{ post.url }}" class="btn zoombtn">Read More</a>
                    </div>
                </div> 
            </div>
        {% cycle 'end row' : nil, '</div>' %}
    {% endfor %}
    {% cycle 'end row' : nil, '</div>' %}
</div>
