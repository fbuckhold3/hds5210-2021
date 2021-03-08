Part 1:  4/5

Looks like there were a couple that you didn't get sorted out on the version turned in.  Let me know if this was just a matter of what was saved versus turned in.


Part 2:  4/5

20.3 - Close.  Initiatilizing those keys with `families['Boal'] = []` etc only works, of course, because you knew ahead of time what they keys needed to be.  The rest of your code is great.  You just need an `if` statement to figure out if the key already exists for the last name that you're looking at inside the loop.  If the key doesn't exist, then create it.  -1

```
for name in names:
  last_name = name[0]
  first_name = name[1]
  
  if families.get(last_name) is None:
    families[last_name] = []
    
  familiise[last_name].append(first_name)
```


20.4 - This setup of a loop within a loop works, but you can also make it simpler (and faster) if you instead of looping over the `avg_los` just retrieve the average length of stay for that particular diagnosis with `avg_los[diagnosis]` and then do your comparison.