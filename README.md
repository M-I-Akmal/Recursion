# Recursion
n=int(input("Masukkan Jumlah Piringan="))
def towerofhanoi_ (x, p, q, r):
    if x==1:
        print("Pindahkan piringan dari", p, "ke", r)
    elif x<=0:
        print("Masukkan jumlah piringan yang valid kaka :)")
    else :
        towerofhanoi_ (x-1,p, r, q)
        print("Pindahkan piringan dari", p,"ke", r)
        towerofhanoi_(x-1, q, p, r)
towerofhanoi_ (n, "p", "q", "r")
