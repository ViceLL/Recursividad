**III.I) Sumatoria de los números del 1 a n : Sum(n)
def Sum(n):**

   if n <= 1:
   
       return n
       
   return n + Sum(n - 1)

n = int(input("Ingrese un numero: "))

print(Sum(n))


**III.II) Factorial de N (1 * 2 * 3 ... * n)
def factorial(n):**

if n == 1:

  return n
  
else:

   return n*factorial(n-1)

num = int(input("Ingrese un numero: "))

print("El factorial de ",num,"es",factorial(num))




**III.III) Máximo común divisor (GCD Euclid's algorithm)**

def gcd(x , y):

  if y == 0:
  
      return x
      
  else:
  
      return gcd(y, x % y)

num_one = int(input("Ingrese un valor para x:"))

num_two = int(input("Enter a value for y:" ))

if num_two == 0:

  print(num_one)
  
else:

  print(gcd(num_one, num_two))



**IV.I) Sumatoria de los números del 1 a n : Sum(n) -> n == 1 ? n : n + Sum(n - 1);**
  
n=int(input("Ingrese un numero: "))

Sum = 0

while(n > 0):

   Sum=Sum+n
   
   n=n-1
   
print("La suma de los números hasta n es",Sum)


**IV.II) Factorial de N (1 * 2 * 3 ... * n) : Factorial(n) -> n <= 1 ? n : n * Factorial(n - 1);**

num = int(input("Ingrese un numero: "))

factorial = 1

for i in range(1,num + 1):

   factorial = factorial*i
   
print("El factorial de",num,"es",factorial)


**IV.IV) Máximo común divisor (GCD Euclid's algorithm) : GCD(x, y) -> y == 0 ? x : GCD(y, x % y);**

def gcd(x, y):

 while(y):
 
     x, y = y, x % y
     
 return x

num_one = int(input("Ingrese un valor para x: "))

num_two = int(input("Ingrese un valor para y: "))

if num_two == 0:

  print(num_one)
  
else:

  print(gcd(num_one, num_two))


