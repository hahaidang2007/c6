import math
a = float(input ("a"))
b = float(input ("b"))
c = float(input ("c"))

if a == 0:
    if b == 0:
        if c == 0:
           print("pt vô số nghiệm")
        else:
           print ("pt vô nghiệm")
    else:
         x = -c / b
         print("pt bậc nhất, nghiệm x=", x)
else:
     delta = b**2 - 4*a*c
     if delta > 0:
         x1 = (-b + math.sqrt(delta)) / (2*a)
         x2 = (-b - math.sqrt(delta)) / (2*a)
         print("pt có 2 nghiệm phân biệt:")
         print("x1 =", x1)
         print("x2 =", x2)
     elif delta == 0:
           x = -b / (2*a)
           print("pt có nghiệm kép x=", x)
     else:
           print("pt vô nghiệm trong tập số thực")
