#Nama Pembuat
print("Nama : Reyfaldho Alfarazel")
print("Nim : 2309116007")
print("---------------------------")
print("masukan nama, nim, dan password ")

def login():
    nama = input("masukan nama : ")
    nim = input("masukan nim : ")
    password = input("masukan password : ") 
    
    if nama == "Reyfaldho Alfarazel" and nim == "2309116007" and password == "sisteminformasijayajaya": 
        print("selamat anda telah login ")
    else:
        print("login gagal,silahkan check nama nim dan password")
login()

print("===========================================================")
print("silahkan kerjakan menghitung rumus segitiga pythagoras ini")
print("1. Sisi Alas")
print("2. Sisi Tegak")
print("3. Sisi Miring")

operasi  =float(input("masukan operasi sisi (1/2/3): "))

import math
if operasi == 1:
    sisi_miring =int(input("masukan Nilai sisi miring: "))
    sisi_tegak =int(input("masukan nilai sisi tegak: "))
    sisi_alas =math.sqrt(sisi_miring**2 - sisi_tegak**2)
    print("hasil dari sisi alas adalah: ",sisi_alas)
elif operasi == 2:
    sisi_miring =int(input("masukan nilai sisi miring: "))
    sisi_alas =int(input("masukan nilai sisi alas: "))
    sisi_tegak= math.sqrt(sisi_miring**2 - sisi_alas**2)
    print("hasil dari sisi tegak adalah: ",sisi_tegak)
elif operasi == 3:
    sisi_alas =int(input("masukan nilai sisi alas: "))
    sisi_tegak =int(input("masukan nilai sisi tegak: "))
    sisi_miring = math.sqrt(sisi_alas**2 + sisi_tegak**2)
    print("hasil dari sisi miring adalah: ",sisi_miring)
else:
    print("operasi tidak tersedia")
