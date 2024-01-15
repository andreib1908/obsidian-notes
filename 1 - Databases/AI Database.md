---
type: database
module: "6"
field 1: computer science - ai
field 2: logic
---
# All Notes

```dataview
table parent, field, short_desc 
where type = "topic" and (module = "6" or module = "4, 6")
SORT file.name ASC
```

# Only Logic

## All logic

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic"
```

## Prop Logic

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic" and field_type = "propositional logic"
```

## Theorem Proving Logic

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic" and field_type = "theorem proving logic"
```

## Predicate logic

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic" and field_type = "predicate logic"
```

## Search Logic

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic" and field_type = "search logic"
```

## Prolog

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "logic" and field_type = "prolog"
```
# Only AI Theory

```dataview
table parent, field_type, short_desc
where type = "topic" and field = "AI"
```


# Only Math

```dataview
table parent, field_type, short_desc
where field = "math" and (module = "6" or module = "4, 6") and type = "topic"
sort file.name asc
```


# Only probabilistic reasoning w3

```dataview
table parent, short_desc
where (field = "AI" or field = "math") and (module = "6" or module = "4, 6") and type = "topic" and (field_type = "probabilistic reasoning" or field_type= "probability")
sort file.name asc
```


# Only machine learning w4

```dataview
table parent, short_desc
where (field = "AI" or field = "math") and (module = "6" or module = "4, 6") and type = "topic" and (field_type = "machine learning")
sort file.name asc
```
- [x] #database 