guests_1 = [ "Bethaney Bain", "Kacey Johns", "Manpreet Saunders" ]
guests_2 = [ "Elwood Curtis", "Diya Griffin", "Kacey Johns" ]
guests_3 = [ "Tobey Weiss", "Kadie Barnes", "Diya Griffin" ]

print("#"*20)
print ("\tGuest List")
guests= guests_1+ guests_2+guests_3 
x =list(set(guests))
x.sort()
for i, x1 in enumerate(x):
    print( i+1,x1, sep=" ")
print("#"*20)
