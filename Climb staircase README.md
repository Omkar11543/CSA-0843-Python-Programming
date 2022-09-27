def sta(n):
    if n<=1:
        return n
    return sta(n-1)+sta(n-2)
def count(s):
    return sta(s+1)
s=int(input("ENTER THE WAYS---> "))
print("THE NUMBER OF WAYS----> ",(count(s)))
