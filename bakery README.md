a=int(input("enter the no of new loaves"))
b=int(input("enter the no of old loaves"))
if(a>=0):
    NL=185*a
    OL=185*b*0.6
    T=OL+NL
    print("the amount of new loaves",NL)
    print("the amount of old loaves",OL)
    print("the total amount",T)
else:
    print("INVALID")
    

