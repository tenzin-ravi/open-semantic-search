---
title: Installation
authors:
    - Markus Mandalka
---

# Installation

# Installation on a desktop computer, laptop or notebook running on Linux, Windows or Mac (desktop search)

Single desktop users can use the preconfigured toolbox bundle and virtual machine [Open Semantic Desktop Search](../../desktop_search).


# Docker

Coming soon.


# Installation on a Linux server or VM (organizations or research teams)

Installation on a Linux server for social search or collaborative research for an organizations or a research team:

[Install Open Semantic Search on a Ubunto or Debian GNU/Linux server](search_server).

I hope it helps people who are unable to make this wonderful product with django 4. Here are the steps I had to take on Debian Bullseye 11.
1. Downgrade django to django 3.2 
sudo pip install Django==3.2.0
2. Migrate the SQL Lite schema.
cd /var/lib/opensemanticsearch/
python3.9 manage.py makemigrations
python3.9 manage.py migrate
