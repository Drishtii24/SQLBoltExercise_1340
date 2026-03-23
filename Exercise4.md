# Exercise_4

## 1. List all directors of Pixar movies (alphabetically), without duplicates

## Query
```sql
     SELECT DISTINCT director
     FROM movies
     ORDER BY director ASC;
```

## Output
| director |
|---|
| Andrew Stanton |
| Brad Bird |
| Brenda Chapman |
| Dan Scanlon |
| John Lasseter |
| Lee Unkrich |
| Pete Docter |

## 2. List the last four Pixar movies released (ordered from most recent to least)

## Query
```sql
     SELECT title, year
     FROM movies
     ORDER BY year DESC
     LIMIT 4;
```

## Output
| title | year |
|---|---|
| Monsters University | 2013 |
| Brave | 2012 |
| Cars 2 | 2011 |
| Toy Story 3 | 2010 |

## 3. List the first five Pixar movies sorted alphabetically

## Query
```sql
     SELECT title
     FROM movies
     ORDER BY title ASC
     LIMIT 5;
```

## Output
| title |
|---|
| A Bug's Life |
| Brave |
| Cars |
| Cars 2 |
| Finding Nemo |

## 4. List the next five Pixar movies sorted alphabetically

## Query
```sql
     SELECT title
     FROM movies
     ORDER BY title ASC
     LIMIT 5 OFFSET 5;
```

## Output
| title | 
|---| 
| Monsters University | 
| Monsters, Inc. | 
| Ratatouille | 
| The Incredibles | 
| Toy Story | 
