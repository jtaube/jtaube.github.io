---
layout: archive
title: "Presentations"
permalink: /presentations/
author_profile: true
---

## Talks

<div>
    {% for deck in site.data.presentations.slides %}
    <figure width="100">
        <a href=
            {% if deck.url contains "://" %}
              "{{ deck.url }}"
            {% else %}
              "{{ deck.url | relative_url }}"
            {% endif %}
            title="{{ deck.title }}"
        >
        <img class="thumb" width="10" src=
          {% if deck.image_path contains "://" %}
            "{{ deck.image_path }}"
          {% else %}
            "{{ deck.image_path | relative_url }}"
          {% endif %}
          alt="{{ deck.title }}">
        </a>
        <figcaption>
        {{deck.title}}
        </figcaption>
    </figure>
    {% endfor %}
</div>

## Posters

<div>
    {% for deck in site.data.presentations.posters %}
    <figure>
        <a href=
            {% if deck.url contains "://" %}
              "{{ deck.url }}"
            {% else %}
              "{{ deck.url | relative_url }}"
            {% endif %}
            title="{{ deck.title }}"
        >
        <img class="thumb" width="10" src=
          {% if deck.image_path contains "://" %}
            "{{ deck.image_path }}"
          {% else %}
            "{{ deck.image_path | relative_url }}"
          {% endif %}
          alt="{{ deck.title }}">
        </a>
        <figcaption>
        {{deck.title}}
        </figcaption>
    </figure>
    {% endfor %}
</div>