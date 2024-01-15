
# Ex1

![[Pasted image 20230912142641.png]]

```python
def get_product_code_index(desired_product, product_codes):  
    # find index  
    index = 0  
    for product in product_codes:  
        if product == desired_product:  
            return index  
        index += 1  
    return -1
```

So, indexes don't increment. The product variable will be the object itself in the list.


i got bored after this :)