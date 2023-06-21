# Trapezoidal-rule

Evaluate ∫
𝟏
𝒅𝒙 using trapezoidal rule with 𝒉 = 𝟎. 𝟐.

Program:
```python
def f(x):
return 1/(1+x**2)
a=float (input ("Enter the lower limit: "))
b=float (input ("Enter the upper limit: "))
h=float (input ("Enter the step size: "))
n=int((b-a)/h)
sum=0
for i in range (1, n):
sum=sum+f(a+i*h)
trap=h/2*(f(a)+f(b)+2*sum)
print ("The Integral value is %.5f"%trap)
```
Output:
Enter the lower limit: 0
Enter the upper limit: 1
Enter the step size: 0.2
The Integral value is 0.78373
