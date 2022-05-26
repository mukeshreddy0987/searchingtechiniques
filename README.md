# searchingtechiniques
#linear searching in datastuctures with python
def linear(li,target):    
    for i in range(len(li)):
        if li[i]==target:
            return i
#binary search with python 
def binarysearch(li,target):
    low=0
    high=len(li)-1
    while low<=high:
        mid=(low+high)//2
        if li[mid]==target:
            return mid
        else:
            if li[mid]>target:
                high=mid
            else:
                low=mid
li=[1,3,5,6,7,8,90,3454,4567,7890,98765]
binarysearch(li,7890)
