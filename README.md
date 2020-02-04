# Removing-repeated-character
str="bacgsdgh"
str1=[]
str2=[]
str3=[]
cnt=0
print(str)
for i in str:
  str1.append(i)
  str2.append(i)
for i in range(0,7):
  for j in range(i+1,7):
    if(str1[i]==str2[j]):
      str1[i]=0
      
for i in str1:
  if(i=='0'):
    str3.append(i)
    
for i in str1:
  if(i!=0):
    str3.append(i)
    
for i in str3:
  if(i=='\n'):
    break
  else:
    cnt=cnt+1
print("Latest count of character after removing repeated one:",cnt)
print("String in sorted order")
print(sorted(str3))
