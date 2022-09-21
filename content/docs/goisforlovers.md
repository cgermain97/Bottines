---
date: "2014-04-02"
tags: ["go", "templates"]
title: "Introduction à Go"
toc: true
---

Hugo utilise l'excellente bibliothèque Go [html/template][gohtmltemplate] pour son moteur de modèles. Il s'agit d'un moteur extrêmement léger qui fournit une très petite quantité de logique. 

Ce document est une brève introduction à l'utilisation des modèles Go. La [documentation Go][gohtmltemplate] fournit plus de détails.

## Syntaxe de base

Les templates Go sont des fichiers HTML avec l'ajout de variables (et de fonctions).

Les variables sont appelées sur ce modèle : 

    {{ .Nom }}

Donc par exemple dans le template html, plutôt que d'écrire le titre de mon site, si j'ai défini le titre de mon site dans le fichier de configuration (config.toml) sous le nom "title", je vais pouvoir appeler la donnée ainsi :

<title>{{ .Title }}</title>

Pour des variables qui sont dans des catégories (notées entre [] dans config.toml). 
Pour appeler la variable "description" dans la catégorie [params], je vais noter dans mon template : 

    {{ .Params.description }}

ou 

    {{ .Site.Params.description }}

Je peux également définir la variable dans son appel : 

    {{ $address := "123 Main St."}}
    {{ $address }}


[go]: https://golang.org/
[gohtmltemplate]: https://golang.org/pkg/html/template/
