---
layout: index
title: Home
comments: false
description: "Hello everybody. This is about Manikanta, an Amateur Astronomer and an easy going comp. science undergrad at Indian Institute of Technology, Kanpur. He isn't much but, yeah, here you go"
---

<center>
	<h2>Hi!</h2>
</center>
Hello everybody. This is about Manikanta, an Amateur Astronomer and an easy going comp. science undergrad at Indian Institute of Technology, Kanpur. I heard that you wanted to know me, so here you go.

<hr class="hr-line">

<center>
	<h2>What interests me?</h2>
</center>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/ml.png">
        </div>
    <h3 class="centered"><b>Machine Learning</b></h3>
    <h3 class="centered"><b>& Data Analysis</b></h3>
        <p>My favorite <i>idle time</i> activity. What's better than to find patterns in everything? The feeling you get when your machine learns something better than you do, is crazy! I was recently working on numerous short projects/ assignments, look them up!</p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/eye.png">
        </div>
        <h3 class="centered"><b>Computer Vision</b></h3>
        <h3 class="centered"><b>& Image Processing</b></h3>
        <p>Image processing and computer vision are interesting topics! Although it takes time, some algorithms are way over the place. I'm currently into trying segmenting nerves in ultra sound images.</p>
    </div>
</div>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/universe.png">
        </div>
        <h3 class="centered"><b>Astro Physics</b></h3>
        <p>I like the dark skies a lot. I spend many nights, just lying there and watch them stars twinkle. I also like cosmology, stellar statistics and studying the large-scale structure of the universe. I guess attending an astronomy-ocsc does have its perks!</p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/music.png">
        </div>
        <h3 class="centered"><b>Music</b></h3>
        <p>I have got a really wanky taste in music, mostly electronic pop. I find it really relaxing to plug in my earphones and dream with volume on full. Stalk on my <a href="http://last.fm/ManikantaReddy">last.fm</a> to see if we match.</p>
    </div>
</div>

<div class="row mt ">
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/food.png">
        </div>
        <H3 class="centered"><b>Food</b></H3>
        <p>
            I can cook too. When I've nothing else to do, you can always find me in the kitchen cooking delicous food and eating it. If I ever invite you over, trust me, it'll be fireworks in your mouth.
        </p>
    </div>
    <div class="col-md-6">
        <div class="centered">
            <img src="assets/img/interests/earth.png">
        </div>
        <h3 class="centered"><b>Everthing Else</b></h3>
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
