# Studi_Kasus_5_Deka-Rizky-Fauzan
# tugas ddp pertemuan 5

def hitung_parkir(kendaraan, jam):
    if kendaraan == "mobil":
        biaya = jam * 5000
    elif kendaraan == "motor":
        biaya = jam * 3000
    else:
        biaya = 0

    return biaya


print("BIAYA PARKIR RS UNMUL")

kendaraan = input("Jenis kendaraan (mobil/motor): ")

masuk = int(input("Jam masuk  : "))
keluar = int(input("Jam keluar : "))

lama = keluar - masuk

hasil = hitung_parkir(kendaraan, lama)

print()
print("Jenis kendaraan :", kendaraan)
print("Jam masuk       :", masuk)
print("Jam keluar      :", keluar)
print("Lama parkir     :", lama, "jam")
print("Biaya parkir    : Rp", hasil)
