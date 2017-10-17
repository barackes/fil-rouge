# Descriptif du dataset

Ce dataset contient les notes des utilisateur par rapport à un film, chaque film à un ou plusieurs genre, ainsi qu'un tag personnel de l'utilisateur pour dire succinctement son idée à propos du film.

## tags.csv:

Le tags.csv, une **associtation** entre un user et un film de telle facon pour chaque pair (user,movie) on a un tag, comporte quatre colone :
1. un userId(de type Long) qui sert a déteminer le user, un movieId (de type Long) qui sert à determiner le film en question, 
2. un tag (de type varchar) qui represente une idée global et personnelle de l'utilisateur à propos du film,
3. un timestamp (de type timestamp) qui represente le moment de la création de cet enregistrement en seconde,

## ratings.csv
	
Le ratings.csv, une **associtation** entre un user et un film de telle facon pour chaque pair (user,movie) a une note, comporte quatre colone 
1. un userId(de type Long) qui sert a déteminer le user,
2. un movieId (de type Long) qui sert à determiner le film en question,
3. un rating qui represente la note que l'utilisateur à donner au film et c'est une valeur allant de 0.5 à 5 (de type float) d'un pas de 0.5, chaque film à necessairement une note,
4. un timestamp qui represente le moment de la création de cet enregistrement en seconde, 

## movies.csv

Le movies.csv comporte trois colone :
1. le movieId, 
2. le titre (de type varchar) qui renseigne le titre du film en question,
3. genres (de type varchar), pour déterminer le genre du film , un film a au moin un genre

## links.csv

Le links.csv comporte trois colone toute des ID, elle relie le meme film entre trois différents base de donnée à savoir du systéme courant, celui de imdb et tmdb

## genome-scores.csv

Le genome-scores.csv comporte trois colone:
1. movieId,
2. tagId,
3. relevance, cette derniére montre à quel point le tag exprime bien le film et ceci par le biais d'un algorithme de machine learning déroulé sur les avis textuelle et note des utilisateur

## genome-tags.csv

Le genome-tags.csv comporte deux colone, tagId et le tag qui décrit le tagId dans le genome file