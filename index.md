---
layout: default
title: "Início"
---

# 👋 Bem-vindo ao meu blog técnico

Aqui compartilho aprendizados sobre **Golang**, **arquitetura de software** e **boas práticas de engenharia**.

Sinta-se à vontade para explorar os posts e deixar feedback!

---

## 📚 Últimos posts

<div class="post-grid">
  {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="post-card">
      <div class="post-content">
        <h3 class="post-title">{{ post.title }}</h3>
        <div class="post-excerpt">{{ post.excerpt | strip_html | truncate: 130 }}</div>
        <div class="post-meta">
          {{ post.date | date: "%d %b %Y" }} · {{ post.categories | join: ", " }}
        </div>
      </div>
    </a>
  {% endfor %}
</div>
