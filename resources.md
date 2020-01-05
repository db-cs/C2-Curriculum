---
# Page settings
layout: default
head_title: Resources
keywords:
comments: false

# Hero section
title: Resources
description: The following tools and resources can be helpful as you work on projects in class. Be sure to explore each resource so that you will know where to find additional information when you need it.

grid_navigation:
    - title: GitHub Student Developer Pack
      excerpt: Free access to the best developer tools in one place so you can learn by doing.
      cta: Check it out
      url: 'https://education.github.com/pack/'
    - title: FreeCodeCamp
      excerpt: Learn to code with free online courses, programming projects, and interview preparation for developer jobs.
      cta: Check it out
      url: 'https://www.freecodecamp.org/'
    - title: Web Developer Roadmap
      excerpt: A Visual Guide to Becoming a Front End, Back End, or DevOps Developer
      cta: Check it out
      url: 'https://www.freecodecamp.org/news/2019-web-developer-roadmap/'

---

<div class="section">
    <div class="container">
        <div class="row">
            <div class="col-md-12">
                <div class="nav-grid nav-grid--out">
                    <div class="row">
                        {% for item in page.grid_navigation %}
                            <div class="col-sm-6 col-lg-4">
                                <a href="{% if jekyll.environment == 'production' %}{{ site.doks.baseurl }}{% endif %}{{ item.url }}" class="nav-grid__item">
                                    <div class="nav-grid__content" data-mh>
                                        <h2 class="nav-grid__title">{{ item.title }}</h2>
                                        <p>{{ item.excerpt }}</p>
                                    </div><!-- /.nav-grid__content -->
                                    <p class="nav-grid__btn">
                                        {{ item.cta }}
                                        <i class="icon icon--arrow-right"></i>
                                    </p>
                                </a><!-- /.nav-grid__item -->
                            </div><!-- /.col -->
                        {% endfor %}
                    </div><!-- /.row -->
                </div><!-- /.nav-grid -->
            </div><!-- /.col -->
        </div><!-- /.row -->
    </div><!-- /.container -->
</div><!-- /.section -->
