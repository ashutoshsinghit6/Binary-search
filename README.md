# Binary-search
def bsearch(a,item):
    beg=0
    last=len(a)-1

    while (beg<=last):
        mid=int((beg+last)/2)
        print(mid)
        if (item==a[mid]):
            return mid
        elif (item>a[mid]):
            beg=mid+1
        else:
            last=mid-1

n=int(input("enter size of array:"))
arra=[int(input()) for i in range (n)]
print(a)
item=int(input("enter search item:"))
index=bsearch(a,item)
if index or index==0:
    print("element found",index)
else:
    print("not found")
