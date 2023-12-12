#Bài 1. Viết chương trình xuất ra màn hình nhiệt độ (oK) tương ứng khi nhập vào nhiệt độ (oC)?
Celsius = float(input("Nhập độ C = "))
Kelvin = Celsius + 273.15
print ("Độ K = ", Kelvin, "K")

#Bài 2: Viết chương nhập vào 2 số nguyên dương m và n (m>n), hãy in ra màn hình phần nguyên và phần dư của m chia cho n?
m = int(input("Nhap m = "))
n = int(input("Nhap n = "))
div = m // n
mod = m % n
print ("Phần nguyên là: ", div, "Phần dư là: ", mod)

#Bài 3. Viết chương trình  Python nhập vào độ dài 2 cạnh của hình chữ nhật, tính chu vi và diện tích hình chữ nhật đó.
a = float (input("Nhập độ dài cạnh thứ nhất:"))
b = float (input("Nhập độ dài canh thứ hai:"))
chuvi = (a + b) * 2
dientich = a * b
print ("Chu vi hình chữ nhật là: ", chuvi)
print ("Dien tich hình chữ nhật là: ", dientich)

#Bài 4. Viết chương trình  Python nhập vào bán kính của hình tròn, tính chu vi và diện tích hình tròn đó.
PI = 3,14
r = float(input("Nhập bán kính hình tròn:"))
C = 2*PI*r
S = C*C / 4 * PI
print ("Chu vi hinh tron la:", C)
print ("Dien tich hinh chu nhat la:", S)

#Bài 5. Viết chương trình  Python nhập vào ba số a,b,c bất kì. Kiểm tra xem 3 số đó có thể  là độ dài ba cạnh tam giác hay không, nếu  không  thì in  ra màn  hình  ‘ Không tạo thành tam giác’. Ngược lại, tính chu vi và diện tích tam giác đó.
from math import sqrt
a = float (input("Nhập độ dài cạnh thứ nhất:"))
b = float (input("Nhập độ dài cạnh thứ hai:"))
c = float (input("Nhập độ dài cạnh thứ ba:"))
if a+b>c and a+c>b and b+c>a:
   cv = a+b+c
   p = (a+b+c)/2
   dt = sqrt(p*(p-a)*(p-b)*(p-c))
   print('Chu vi = {0}'.format(cv))
   print('Dien tich = {0}'.format(dt))
else: print('Không tạo thành tam giác')

#Bài 6. Viết chương trình nhập ba số nguyên dương a, b, h từ bàn phím lần lượt là độ dài đáy lớn, đáy bé và chiều cao của một hình thang. Tính diện tích hình thang và in kết quả ra màn hình.
from math import sqrt
a = float(input("Nhập a = "))
b = float(input("Nhập b = "))
h = float(input("Nhập h = "))
DT = (a + b) * h / 2
print("Diện tích hình thang là:", DT)
