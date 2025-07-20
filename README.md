# Petit-script-avec-Maps-
Utiliser la bibliothèque maps pour ressortir un pays a partir de la carte du monde
---
title: "utilisation maps personnelle"
author: "IVANE"
date: "2025-07-20"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

# chargement de la bibliotheque
```{r}
library(maps)
```

# tracer une carte simple du monde
```{r}
map("world")
```

# carte d un pays d afrique (cas du Gabon)
```{r}
map("world", regions = "Gabon")
```

# en difinissant la latitude et la lomgitude
```{r}
map("world", xlim = c(10, 25), ylim = c(-5, 15), fill = TRUE, col = "lightblue")
```

# pour le cameroun
```{r}
map("world", xlim = c(8,17), ylim = c(1,14), fill = TRUE, col = "lightblue")
title("zoom sur le cameroun")
```
# zoom sur une ville du cameroun
```{r}
map("world", xlim = c(13.5, 15.5), ylim = c(9.5, 11.5), fill = TRUE, col = "lightyellow", bg = "lightblue")
text(14.324, 10.595, labels = "Maroua", pos = 3, col = "red")
title("zoom sur Maroua - Cameroun")
```

