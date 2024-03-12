n=int(input())
d={}
for i in range(1,n+1):
  d[i]=[]
  for j in range(1,i+1):
    if i%j==0:
      d[i].append(j)
d1={}
for i in d:
  if len(d[i])>2:
    d1[i]="not Prime"
  else:
    d1[i]="Prime"
print(d1)
