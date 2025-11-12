# 28
код10
f = open('27.txt')
n = int(f.readline())
k = int(f.readline())
a = [int(x) for x in f]
st = 10**10
fin = 10**10
proizved = 10**10
for i in range(2*k,n):
    st = min(st, a[i-2*k])
    fin = min(fin, st * a[i-k])
    proizved = min(proizved, fin * a[i])
print(proizved)
