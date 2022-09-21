---
title: "Shortcodes"
date: 2019-02-12T23:39:06-06:00
tags: [shortcodes]
toc: true
---

## Bloc de citation

```
{{</* blockquote author="Alan Turing" */>}}
La science ne nous dit pas où nous allons - c’est le rôle de l’art - ; elle nous dit où nous sommes.
{{</* /blockquote */>}}
```

{{< blockquote author="Alan Turing" >}}
La science ne nous dit pas où nous allons - c’est le rôle de l’art - ; elle nous dit où nous sommes.
{{< /blockquote >}}

## Note

```
{{</* note */>}}
C'est une note ! Une note qui peut être *balisée* en `markdown`. 
{{</* /note */>}}
```

{{< note >}}
C'est une note ! Une note qui peut être *balisée* en `markdown`. 
{{< /note >}}

## Expansion

{{< expandable label="expansion 1" level="2" >}}
Texte
{{< /expandable >}}

{{< expandable label="expansion 2" level="2" >}}
Texte
{{< /expandable >}}

{{< expandable label="expansion 3" level="2" >}}
Texte
{{< /expandable >}}

## Arborescence

```
{{</* fileTree */>}}
* Niveau 1  
    * Section 1
    * Section 2 
        * Sous-section 1
        * Sous-section 2
            * Sous-sous-section 1
        * Sous-section 3
            * Sous-sous-section 1  
            * Sous-sous-section 2   
    * Section 3  
        * Sous-section 1  
        * Sous-section 2  
        * Sous-section 3    
* Niveau 2  
{{</* /fileTree */>}}
```

{{< fileTree >}}
* Niveau 1  
    * Section 1
    * Section 2 
        * Sous-section 1
        * Sous-section 2
            * Sous-sous-section 1
        * Sous-section 3
            * Sous-sous-section 1  
            * Sous-sous-section 2   
    * Section 3  
        * Sous-section 1  
        * Sous-section 2  
        * Sous-section 3    
* Niveau 2  
{{< /fileTree >}}

## Image

```
{{</* figureCupper
img="image.jpg" 
caption="Légende avec crédits" 
command="Resize" 
options="700x" */>}}
```

{{< figureCupper
img="image.jpg" 
caption="Légende avec crédits" 
command="Resize" 
options="700x" >}}