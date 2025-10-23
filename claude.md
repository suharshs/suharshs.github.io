# Anisha & Suharsh Restaurant Review Blog

A Jekyll-based restaurant review blog hosted on GitHub Pages, featuring a unique 100-point rating system for restaurant reviews.

## Overview

This is a personal blog maintained by Anisha and Suharsh, focused on providing detailed restaurant reviews with a custom category-based scoring system. The blog challenges traditional 1-5 star ratings by offering more granular, category-specific evaluations.

**Live Site**: [anishasuharsh.com](http://anishasuharsh.com)

## Project Structure

```
suharshs.github.io/
├── _config.yml           # Jekyll configuration
├── _includes/            # Reusable HTML components
│   ├── footer.html
│   ├── header.html
│   ├── head.html
│   ├── rating_chart.html
│   └── social.html
├── _layouts/             # Page templates
│   ├── default.html
│   ├── home.html
│   ├── page.html
│   └── post.html
├── _posts/               # Blog posts (restaurant reviews)
├── _site/                # Generated static site
├── about.markdown        # About page with rating methodology
├── index.markdown        # Home page
├── 404.html             # Custom 404 page
├── CNAME                # Custom domain configuration
├── Gemfile              # Ruby dependencies
└── Gemfile.lock         # Locked dependency versions
```

## Rating System

The blog uses a 100-point rating system with the following categories:

- **Yumminess (60 points)**: Taste and flavor of the food
- **Quality (15 points)**: Ingredient quality and preparation
- **Service (10 points)**: Customer service experience
- **Value (10 points)**: Price-to-quality ratio
- **Ambiance (5 points)**: Restaurant atmosphere

## Technology Stack

- **Static Site Generator**: Jekyll 4.x
- **Theme**: Minima (~2.5)
- **Hosting**: GitHub Pages
- **Domain**: Custom domain via CNAME (anishasuharsh.com)
- **Plugins**:
  - jekyll-feed (RSS feed generation)

## Post Structure

Each restaurant review post includes:

```markdown
---
layout: post
title: "Restaurant Name"
date: YYYY-MM-DD HH:MM:SS -0700
categories: ["Location", "Cuisine Type"]
yumminess: 0-60
quality: 0-15
value: 0-10
service: 0-10
ambiance: 0-5
---

## What We Ordered
- Dish 1
- Dish 2

## Our Review
Detailed review text...
```

## Current Reviews

The blog currently features reviews of restaurants in the Bay Area/South Bay, CA, including:

- **Thai**: Dusita Thai, Old Siam, Sri Vasantha Bhavan
- **Mexican**: Casa Lupe, Margaritas Taqueria
- **Pizza**: Cicero's Pizza
- **Ramen**: Ramen Izakaya

## Local Development

To run the site locally:

```bash
# Install dependencies
bundle install

# Serve the site locally
bundle exec jekyll serve

# Site will be available at http://localhost:4000
```

## Deployment

The site is automatically deployed via GitHub Pages when changes are pushed to the main branch.

## Philosophy

The blog was created to address two main problems with traditional review sites:

1. **Simplistic Ratings**: 1-5 star systems lack nuance and specificity
2. **Lack of Context**: Reviews often don't clarify the reviewer's perspective and preferences

By providing detailed category scores and comprehensive reviews, the blog aims to help readers determine if a restaurant matches their specific preferences, regardless of whether their tastes align with the reviewers'.

## Content Guidelines

When adding new restaurant reviews:

1. Create a new file in `_posts/` with the format: `YYYY-MM-DD-restaurant-name.markdown`
2. Include all required front matter fields (layout, title, date, categories, ratings)
3. List dishes ordered under "## What We Ordered"
4. Provide detailed review under "## Our Review"
5. Be honest about both positives and negatives
6. Include specific details that help readers make informed decisions

## Contributing

This is a personal blog, but if you'd like to suggest improvements or corrections, please open an issue or submit a pull request.

## License

Copyright © 2023 anishasuharsh.com
