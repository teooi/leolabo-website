---
layout: page
title: Decoding Brain to Visualize Sleep
permalink: /projects/
toggle: on
rank: 1
---
<p>Neuroimaging through functional Magnetic Resonance Imaging (fMRI) has significantly enhanced our understanding of the brain. However, the challenge of visualizing dreams remains unresolved. <em>Leolabo's Decoding Brain to Visualize Sleep</em> project aims to address this challenge by developing an advanced fMRI model designed to decode and visualize cognitive experiences during sleep.

To realize this vision, we will develop a model capable of detecting and interpreting what an individual sees or imagines. This process will be structured in phases, with the model being trained to recognize and interpret objects, letters, and faces.

This project enables a deeper understanding of how visual information is stored in the brain, provides greater insight into the subconscious mind, and advances the development of machine learning algorithms. 
Potential applications include enhancing criminal investigations by detecting intrusive thoughts and improving the accuracy of understanding a person's mental state during interrogations. Additionally, this technology could enhance communication for non-verbal individuals by providing a way to understand their thoughts and intentions, improving interactions with caregivers.
</p>
<div class="lab-wrapper">
    <ul class="lab-list">
    {% for project in site.data.projects %}
    {% if project.name and project.description %}
        <li>
            <h2>{{ project.name }}</h2>
            {% if project.photo %}
                <img class="float-right projects-photo" src="{{ project.photo | prepend: site.images_dir | prepend: site.baseurl }}">
            {% endif %}
            {% if project.funding %}
                <p><b>Funding: </b>{{ project.funding }}</p>
            {% endif %}
            {% if project.collaborators %}
                <p><b>Collaborators: </b>{{ project.collaborators }}</p>
            {% endif %}
            {% if project.assignees %}
                <p><b>Assignees: </b>{{ project.assignees }}</p>
            {% endif %}
            <p>{{ project.description }}</p>
        </li>
    {% endif %}
    {% endfor %}
    </ul>
</div>
