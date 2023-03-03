---
title: Kids Cup of Rochester
layout: default
---

<section id="intro">
    <div class="background-image" style="background-image: url('{{ site.intro.image }}');"></div>
</section>
<section id="quick-actions">
    <div class="container">
        <div class="item flex-33 flex-100-tablet is-center-aligned has-gutter">
            <a class="is-button" href="{{ site.quick_actions.want_to_golf.button_link }}" target="_blank">
                <span class="fas fa-golf-ball fa-lg is-icon"></span>
                {{ site.quick_actions.want_to_golf.button_text }}
            </a>
        </div>
        <div class="item flex-33 flex-100-tablet is-center-aligned has-gutter">
            <a class="is-button" href="{{ site.quick_actions.want_to_donate.button_link }}" target="_blank">
                <span class="fas fa-donate fa-lg is-icon"></span>
                {{ site.quick_actions.want_to_donate.button_text }}
            </a>
        </div>
        <div class="item flex-33 flex-100-tablet is-center-aligned has-gutter">
            <a class="is-button" href="{{ site.quick_actions.want_to_sponsor.button_link }}">
                <span class="fas fa-handshake fa-lg is-icon"></span>
                {{ site.quick_actions.want_to_sponsor.button_text }}
            </a>
        </div>
        <!--<div class="item flex-25 flex-50-tablet is-center-aligned has-gutter">
            <a class="is-button" href="{{ site.quick_actions.want_to_purchase_tickets.button_link }}">
                <span class="fas fa-ticket-alt fa-lg is-icon"></span>
                {{ site.quick_actions.want_to_purchase_tickets.button_text }}
            </a>
        </div>-->
    </div>
</section>
<section id="event-details" class="has-light-gray-background">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Next Event</h3>
        </div>
        <div class="item flex-50 is-center-aligned">
            <span class="fa fa-calendar-alt fa-2x is-icon"></span>
            <h4>Date & Time</h4>
            <p>
                {{ site.next_event.date | date: '%B %d, %Y' }}
                <br>
                {{ site.next_event.time }}
            </p>
        </div>
        <div class="item flex-50 is-center-aligned">
            <span class="fa fa-map-marker-alt fa-2x is-icon"></span>
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
            <h3 class="is-center-aligned is-section-heading">Who We Are</h3> <img class="is-floated-right"
                src="{{ site.who_we_are.image }}" /> {{ site.who_we_are.text | markdownify }}
        </div>
    </div>
</section>
<section id="whats-new">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">What's New </h3> <img class="is-floated-right"
                src="{{ site.whats_new.image }}" /> {{ site.whats_new.text | markdownify }}
        </div>
    </div>
</section>
<section id="sponsors" class="has-light-gray-background">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading no-bottom-margin">Sponsors</h3>
        </div>
        <div class="item flex-100">
            <div class="container is-full-width has-centered-items has-no-padding">
                <div class="item flex-100">
                    <h4 class="is-center-aligned is-subsection-heading">Presenting Sponsors</h4>
                </div> {% for sponsor in site.presenting_sponsors %} <div
                    class="item flex-33 flex-50-tablet has-padding-two has-gutter has-centered-content has-white-background">
                    <a href="{{ sponsor.link}}" target="_blank" class="item-overlay-link"></a> <img
                        src="{{ sponsor.image }}" class="has-no-margins" /> </div> {% endfor %}
            </div>
        </div>
        <div class="item flex-100">
            <div class="container is-full-width has-centered-items has-no-padding">
                <div class="item flex-100">
                    <h4 class="is-center-aligned is-subsection-heading">Corporate Sponsors</h4>
                </div> {% for sponsor in site.corporate_sponsors %} <div
                    class="item flex-25 flex-33-tablet has-padding-two has-gutter has-centered-content has-white-background">
                    <a href="{{ sponsor.link}}" target="_blank" class="item-overlay-link"></a> <img
                        src="{{ sponsor.image }}" class="has-no-margins" /> </div> {% endfor %}
            </div>
        </div>
        <div class="item flex-100">
            <div class="container is-full-width has-centered-items has-no-padding">
                <div class="item flex-100">
                    <h4 class="is-center-aligned is-subsection-heading">Event Sponsors</h4>
                </div> {% for sponsor in site.event_sponsors %} <div
                    class="item flex-25 flex-33-tablet has-padding-two has-gutter has-centered-content has-white-background">
                    <a href="{{ sponsor.link}}" target="_blank" class="item-overlay-link"></a> <img
                        src="{{ sponsor.image }}" class="has-no-margins" /> </div> {% endfor %}
            </div>
        </div>
        <div class="item flex-100">
            <div class="container is-full-width has-centered-items has-no-padding">
                <div class="item flex-100">
                    <h4 class="is-center-aligned is-subsection-heading">Marketing Sponsors</h4>
                </div> {% for sponsor in site.marketing_sponsors %} <div
                    class="item flex-20 flex-33-tablet has-padding-two has-gutter has-centered-content has-white-background">
                    <a href="{{ sponsor.link}}" target="_blank" class="item-overlay-link"></a> <img
                        src="{{ sponsor.image }}" class="has-no-margins" /> </div> {% endfor %}
            </div>
        </div>
    </div>
</section>
<section id="sign-up">
    <div class="container">
        <div class="item flex-100">
            <h3 class="is-center-aligned is-section-heading">Sign Up</h3>
        </div>
        <div class="item flex-50 has-gutter is-center-aligned"> <span class="fas fa-golf-ball fa-2x is-icon"></span>
            <h4>For Golfers</h4> {{ site.sign_up.for_golfers.text | markdownify }} <p><a class="is-button"
                    href="{{ site.sign_up.for_golfers.button_link }}"
                    target="_blank">{{ site.sign_up.for_golfers.button_text }}</a></p>
        </div>
        <div class="item flex-50 has-gutter is-center-aligned">
            <span class="far fa-handshake fa-2x is-icon"></span>
            <h4>For Sponsors</h4> {{ site.sign_up.for_sponsors.text | markdownify }} <p><a class="is-button"
                    href="{{ site.sign_up.for_sponsors.button_link }}">{{ site.sign_up.for_sponsors.button_text }}</a>
            </p>
        </div>
    </div>
</section>