---
layout: default
---

<section id="intro">
    <div class="background-image" style="background-image: url('uploads/golf_course.jpg');"></div>
    <section id="intro-content">
        <img class="icon" src="assets/images/kids_cup_logo.png">
        <h1 class="title">Kid's Cup Rochester</h1>
    </section>
</section>
<section id="event-details" class="has-light-gray-background">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Next Event</h3>
        </div>
        <div class="item flex-50 is-center-aligned">
            <span class="fa fa-calendar fa-2x is-icon"></span>
            <h4>Date & Time</h4>
            <p>
                {{ site.next_event.date | date: '%B %d, %Y' }}
                <br>
                {{ site.next_event.time }}
            </p>
        </div>
        <div class="item flex-50 is-center-aligned">
            <span class="fa fa-map-marker fa-2x is-icon"></span>
            <h4>Location</h4>
            <p>
                Somerby Golf Club
                <br>
                (<a href="{{ site.next_event.directions_url }}" target="_blank">Directions</a>)
            </p>
        </div>
    </div>
</section>
<section id="who-we-are">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Who We Are</h3>
            <img class="is-floated-right flex-50" src="{{ site.baseurl }}{{ site.who_we_are.image }}" />
            {{ site.who_we_are.text | markdownify }}
        </div>
    </div>
</section>
<section id="what-makes-us-unique" class="has-light-gray-background">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">What Makes Us Unique</h3>
            <img class="is-floated-right flex-50" src="{{ site.baseurl }}{{ site.what_makes_us_unique.image }}" />
            {{ site. what_makes_us_unique.text | markdownify }}
        </div>
    </div>
</section>
<section id="whats-new">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">What's New for 2018</h3>
            <img class="is-floated-right flex-50" src="{{ site.baseurl }}{{ site.whats_new.image }}" />
            {{ site.whats_new.text | markdownify }}
        </div>
    </div>
</section>
<section id="sponsors" class="has-light-gray-background">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Sponsors</h3>
        </div>
        {% for sponsor in site.sponsors %}
            <div class="item flex-33 flex-50-tablet has-padding-two has-gutter has-centered-content has-white-background">
                <a href="{{ sponsor.link}}" target="_blank" class="item-overlay-link"></a>
                <img src="{{ site.baseurl }}{{ sponsor.image }}" class="has-no-margins" />
            </div>
        {% endfor %}
    </div>
</section>
<section id="sign-up">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Sign Up</h3>
        </div>
        <div class="item flex-50 has-gutter is-center-aligned">
            <span class="fa fa-flag fa-2x is-icon"></span>
            <h4>For Golfers</h4>
            {{ site.sign_up.for_golfers.text | markdownify }}
            <p><a class="is-button" href="{{ site.sign_up.for_golfers.button_link }}" target="_blank">{{ site.sign_up.for_golfers.button_text }}</a></p>
        </div>
        <div class="item flex-50 has-gutter is-center-aligned">
            <span class="fa fa-handshake-o fa-2x is-icon"></span>
            <h4>For Sponsors</h4>
            {{ site.sign_up.for_sponsors.text | markdownify }}
            <p><a class="is-button" href="{{ site.sign_up.for_sponsors.button_link }}">{{ site.sign_up.for_sponsors.button_text }}</a></p>
        </div>
    </div>
</section>