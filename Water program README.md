def wc(d,a):
    area=0
    for i in range(a):
        for j in range(i+1,a):
            area=max(area,min(d[j],d[i])*(j-1)) 
            return area
arr=[]
n=int(input("enter the number of element"))
for i in range(0,n):
   ele=int(input("enter the elements"))
   arr.append(ele)
s=len(arr)
print(wc(arr,s))
