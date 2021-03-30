Part 1: 5/5

Part 2: 5/5

I want to point out something in your 30.4.  You have a loop to go through the manifestations and then you check to see if the manifestion is the same as the first one.

```
            for m in manifestation:
                if m == manifestation[0]:
                    manifest = m.get('text')
                else:
                    pass
```

Instead of having that loop, you could also have just said "give me the text for the first manifestation":

```
manifest = manifestation[0].get('text')
```

