--- 
title: Rick and Morty Characters
layout: layout.liquid
pagination:
    data: characters
    size: 1
    alias: character
permalink: '/characters/{{character.name|slug}}/'
---

[//]: # "note, the change in character.data.title from blog cause our new 'template' is a character"


# {{character.name}}

![{{character.name}}]({{character.image}})

ALL OF DA CHARACTERS 
