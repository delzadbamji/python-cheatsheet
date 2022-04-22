# python-cheatsheet
- sort using key1 first then key2
sorted(List[List], key=lambda x: (x[0], x[1]))

   - eg. 1 costs = [[10,20],[30,200],[400,50],[30,20]]
  
  sorted(costs, key=lambda x: (x[0], x[1])) 
  
  > [[10, 20], [30, 20], [30, 200], [400, 50]]
  
  sort by 0th element of sublist, then 1st
  
   - eg2. 
  
     sorted(arr, key=lambda x: (length(x), x))
  
     sort by length and then by value (i.e x)
  
- lambda func (like anonymous function of JS)
  
   - eg. add = lambda a, b : a + b
  
     add(3,6)
  
- sort dictionary by value
  
  sorted(dict1, key=dict1.get)
  
  - eg. d = {'a':4,'b':1,'c':2}
    
    sorted(d,key=d.get)
    
    > {'b':1,'c':2,'a':4}

- sort dictionary by value descending then key ascending
  
  sorted(dict.items(), key=lambda x: (-x[1], x[0]))
  
- if a key exists in a dict, return the value or return the default value
   
  - example 1.
     d = {"a":123,"b":456}
     
     p = d.setdefault("c",111)
     
     p has the value 111 since key c doesn't exist. d is updated to  {"a":123,"b":456, "c":111}
     
  - example 2.
     d = {"a":123,"b":456,"c":789}
     
     p = d.setdefault("c",111)
     
     p has the value 789 since key c exists. d stays same.
  
  
  
