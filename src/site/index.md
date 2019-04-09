---
title: Visual Framework 11ty boilerplate
subtitle: No homepage, yet.
date: 2018-08-22 12:24:50
layout: layouts/base.njk
---

<section class="vf-intro | embl-grid embl-grid--has-centered-content">
<div>
  <!-- empty -->
</div>
<div>
  <h1 class="vf-intro__heading vf-intro__heading--has-tag">👋 It works! <a href="" class="vf-badge vf-badge--primary vf-badge--phases">alpha</a></h1>
  <p class="vf-lede">You've successfully installed the Eleventy boilerplate for Visual Framework 2.0.</p>

  <p class="vf-intro__text">This allows you to use the <a class="vf-link" href="https://www.11ty.io">11ty</a> static site generator with direct access to Visual Framework 2.0 components.

  (coming soon: dynamic building of just the VF 2.0 CSS and JS in use.)</p>
</div>
</section>


## What you get

- the Eleventy static site generator
- access to the Visual Framework component system

To add a component you can use npm/Yarn or install it manually.

### Component installation

- installation: `yarn add @visual-framework/vf-logo`
- updating: `yarn upgrade-interactive --latest`

### Manual installation for customisation

1. Download a pattern
2. Copy it to `./src/components/vf-component-name`

In either case you'll need to re-run `gulp dev` to access the pattern.

### Add your own local component

You can add a custom VF-compatible component to `./src/components` and use it in
your site.

You'll find a `vf-sample` component there, we've used it below:

<div class="vf-box">
{% verbatim %}
Code: {% render "@vf-sample", {text: "with some text"} %}
{% endverbatim %}

Returns: {% render "@vf-sample", {text: "with some text"} %}
</div>
