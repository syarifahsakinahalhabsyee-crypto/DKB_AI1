#Kira Purata Markah
df["Status"] = np.where(df["Markah"] >= 66, "Lulus", "Gagal")

print(df)
pelajar_cemerlang = df[df{"Markah"} >= 80]
print(pelajar_cemerlang)
#Tambah Lajur Gred
import pandas as pd

# For demonstration purposes, creating a dummy DataFrame 'df'.
# In a real scenario, you would load your actual data into 'df' from a file (e.g., CSV).
df = pd.DataFrame({'Markah': [85, 70, 45, 90, 60]})

def tentukan_gred(markah):
  if markah >= 80:
   return "A"
  elif markah >= 65:
   return "B"
  elif markah >= 50:
   return "C"
  else:
   return "D"

df["Gred"] = df["Markah"].apply(tentukan_gred)
print(df)


