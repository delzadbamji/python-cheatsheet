# python-cheatsheet
- sort using key1 first then key2
sorted(List[List], key=lambda x: (x[0], x[1]))

  eg. 1 costs = [[10,20],[30,200],[400,50],[30,20]]
  sorted(costs, key=lambda x: (x[0], x[1])) > [[10, 20], [30, 20], [30, 200], [400, 50]]
  sort by 0th element of sublist, then 1st
  
  eg2. 
  sorted(arr, key=lambda x: (length(x), x))
  sort by length and then by value (i.e x)
  
- lambda func (like anonymous function of JS)
  add = lambda a, b : a + b
  add(3,6)
