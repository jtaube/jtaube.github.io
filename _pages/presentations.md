---
layout: archive
title: "Presentations"
permalink: /presentations/
author_profile: true
---

## Talks

<div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: left;">
    {% for deck in site.data.presentations.slides %}
    <figure style="margin: 0; text-align: left; max-width: 30%;">
        <a href=
            {% if deck.url contains "://" %}
              "{{ deck.url }}"
            {% else %}
              "{{ deck.url | relative_url }}"
            {% endif %}
            title="{{ deck.title }}"
        >
        <img src=
          {% if deck.image_path contains "://" %}
            "{{ deck.image_path }}"
          {% else %}
            "{{ deck.image_path | relative_url }}"
          {% endif %}
          alt="{{ deck.title }}"
          style="width: 100%; height: auto;">
        </a>
        <figcaption>{{ deck.title }}</figcaption>
    </figure>
    {% endfor %}
</div>

<!-- <div>
    {% for deck in site.data.presentations.slides %}
    <figure>
        <a href=
            {% if deck.url contains "://" %}
              "{{ deck.url }}"
            {% else %}
              "{{ deck.url | relative_url }}"
            {% endif %}
            title="{{ deck.title }}"
        >
        <img style="max-width: 30%; height: auto; margin: 10px;" src=
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
</div> -->

## Posters

<div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: left;">
    {% for deck in site.data.presentations.posters %}
    <figure style="margin: 0; text-align: left; max-width: 30%;">
        <a href=
            {% if deck.url contains "://" %}
              "{{ deck.url }}"
            {% else %}
              "{{ deck.url | relative_url }}"
            {% endif %}
            title="{{ deck.title }}"
        >
        <img src=
          {% if deck.image_path contains "://" %}
            "{{ deck.image_path }}"
          {% else %}
            "{{ deck.image_path | relative_url }}"
          {% endif %}
          alt="{{ deck.title }}"
          style="width: 100%; height: auto;">
        </a>
        <figcaption>{{ deck.title }}</figcaption>
    </figure>
    {% endfor %}
</div>

<!-- <div>
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
</div> -->