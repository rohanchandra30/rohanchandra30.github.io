---
layout: blog
name: Grad School Application Help
description: This mini blog can be used by future MS aspirants
---

<section id="grad" class="container content-section text-center">
    <div class="row">
    <h1>GRAD</h1>
        <div class="col-lg-8 col-lg-offset-2">

          <ul class="grad_list">
            {% for grad in site.grad %}
              <li class="grad">
                          <a href="{{ grad.url }}"><h4>{{ grad.name }}</h4></a>
                          <p>
                          {{ grad.description }}
                          </p>
              </li>
            {% endfor %}
          </ul>
        </div>
    </div>
</section>