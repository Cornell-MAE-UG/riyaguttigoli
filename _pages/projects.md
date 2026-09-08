---
layout: default
title: Riya Guttigoli - Portfolio
permalink: /projects/
---

<section class="projects-page">

  <div class="projects-header">
    <h1>Engineering Projects</h1>

    <p>
      Explore my work across robotics, hardware development, energy systems,
      modeling, research, and technology commercialization.
    </p>
  </div>

  <div class="project-filters" aria-label="Filter projects">

    <button
      type="button"
      class="filter-button active"
      data-filter="all">
      All Projects
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="robotics">
      Robotics
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="energy">
      Energy
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="hardware">
      Hardware
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="modeling">
      Modeling
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="research">
      Research
    </button>

    <button
      type="button"
      class="filter-button"
      data-filter="entrepreneurship">
      Entrepreneurship
    </button>

  </div>

  <div class="project-gallery">

    {% assign sorted_projects = site.projects | sort: "order" %}

    {% for project in sorted_projects %}

      <article
        class="gallery-item project-card"
        data-categories="{{ project.categories | join: ' ' | downcase }}">

        <a href="{{ project.url | relative_url }}">

          <div class="project-card-image-wrapper">
            <img
              src="{{ project.image | relative_url }}"
              alt="{{ project.title }}">
          </div>

          <h2 class="project-card-title">
            {{ project.title }}
          </h2>

          {% if project.card_tags %}
            <div class="project-card-tags">
              {% for tag in project.card_tags %}
                <span class="project-tag">{{ tag }}</span>
              {% endfor %}
            </div>
          {% endif %}

        </a>

      </article>

    {% endfor %}

  </div>

</section>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const filterButtons = document.querySelectorAll(".filter-button");
    const projectCards = document.querySelectorAll(".project-card");

    filterButtons.forEach(function (button) {
      button.addEventListener("click", function () {
        const selectedFilter = button.dataset.filter;

        filterButtons.forEach(function (otherButton) {
          otherButton.classList.remove("active");
        });

        button.classList.add("active");

        projectCards.forEach(function (card) {
          const categories = card.dataset.categories
            .split(" ")
            .filter(Boolean);

          const shouldShow =
            selectedFilter === "all" ||
            categories.includes(selectedFilter);

          card.classList.toggle("project-hidden", !shouldShow);
        });
      });
    });
  });
</script>