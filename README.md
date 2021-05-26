# hello-world
This repository contains the code with which I practiced while learning python from scratch
# n = int(input("Enter a number"))
#
# if n > 0:
#    print("Positive")
# elif n == 0:
#    print("Zero")
# else:
#    print("Negative")
#
########################################################################################################################
#
# a = int(input("Enter a number"))
# b = int(input("Enter a number"))
# c = int(input("Enter a number"))
# d = int(input("Enter a number"))
#
# if a >= b and a >= c and a >= d:
#    print(a)
# elif b >= c and b >= a and b >= d:
#    print(b)
# elif c >= a and c >= b and c >= d:
#    print(c)
# else:
#    print(d)
#
########################################################################################################################
#
# a = int(input("Nandu"))
# b = int(input("Rock"))
# i = 1
#
# while i <= a:
#    print("nandu", end = "")
#    j = 1
#    while j < b:
#        print(" rock", end="")
#        j = j + 1
#    if j == b:
#        print(" rock")
#    i = i+1
#
########################################################################################################################
#
# i = 1
# while i <= 100:
#     if i % 3 != 0 and i % 5 != 0:
#         print(i)
#     i = i+1
#
########################################################################################################################
#
# i = 1
# while i <= 4:
#    print("#", end="")
#    j = 1
#    while j < 5:
#        print("#", end="")
#        j += 1
#    if j == 5:
#        print("#")
#    i += 1
########################################################################################################################
# # Practice Printing K
# v = 5
# for i in range(v-1,0,-1):
#     print("*", end = "")
#     for k in range(i):
#         print(" ", end = "")
#     print("*")
# for i in range(v):
#     print("*", end = "")
#     for k in range(i):
#         print(" ", end = "")
#     print("*")
########################################################################################################################
#
# i=1
# for i in range(1,1000,2):
#    print(i)
#
########################################################################################################################
#
# import math as m
# for i in range(1,5000):
#    if m.sqrt(i) % 1 == 0:
#        print(i)
#
########################################################################################################################
#
# candies = 10
# requested = int(input("How many candies do you want?"))
#
# for i in range(requested):
#     if requested > candies:
#         break
#     print("candie")
# if requested > candies:
#     print(candies * "Candie\n")
#     print("Sorry\nOut of stock")
# print("Bye \nHave a nice day")
########################################################################################################################
#
# for i in range(4):
#     for j in range(4-i):
#         print(j+i+1,end="")
#     print()
#
########################################################################################################################
#
# str1='ABCD'
# str2='PQR'
# for i in range(4):
#      print(str1[ : i+1 ] + str2[ i : ])
#
########################################################################################################################
# we can use for else
# nums = [12,23,43,4,56,76,78,89,9]
# for n in nums:
#      if n % 5 == 0:
#           print(n )
#           break
# else:
#      print("Not found")
#
########################################################################################################################
# prime numbers in between
#
# n = int(input("Enter starting number"))
# m = int(input("Enter ending number"))
# print("prime numbers from",n,"to",m,"are")
# for j in range(n, m+1):
#      for i in range(2,j):
#           if j%i == 0:
#                break
#      else:
#           print(j)
########################################################################################################################
# from array import array
# vals = array('i',[12,23,34,54,56,87,89,57,533,45])
# print("There are",len(vals), "integers in the array")
# for i in range (0,len(vals)):
#     print(vals[i])
# newArr = array(vals.typecode, (e for e in vals))
# print(newArr)
# i = 0
# while i < len(vals):
#     print(vals[i])
#     i += 1
########################################################################################################################
# from array import*
# len = int(input("How many numbers do u want to assign"))
# arr = array('i',[])
# x = int(input("First number"))
# arr.append(x)
# for i in range(len - 1):
#     y = int((input("Next number")))
#     arr.append(y)
# print(arr)
# q = int(input("Enter number to search"))
# for x1 in range(len):
#     if q == arr[x1]:
#         print(x1)
#         break
# else:
#     print("Not found")
########################################################################################################################
# from numpy import *
# arr1 = array([1,2,3,4,5])
# print(arr1)
# for a in range(len(arr1)):
#     arr1[a] **= 5
# print(arr1)
# # vectorised operation
# arr2 = array([5,4,3,2,1])
#
# arr3 = arr1 * arr2
# print(arr1, "\n", arr2, "\n", arr3)
########################################################################################################################
# from numpy import *
# print("Normal copy")
# a1 = array([1,2,3,4])
# a2 = a1
# print(id(a1), a1)
# print(id(a2), a2)
#
# print("Shallow copy")
# ar1 = array([1,2,3,4,5,6])
# ar2 = ar1.view()
# ar1[1] = 123
# print(id(ar1), ar1)
# print(id(ar2), ar2)
#
# print("Deep copy")
# arrr1 =array([1,2,3,4,5,6])
# arrr2 = arrr1.copy()
# arrr1[2] = 123
# print(id(arrr1), arrr1)
# print(id(arrr2), arrr2)
########################################################################################################################
# # Code for finding greatest number in the array
# from numpy import *
# arr = array([1,2,3,4,5,6,7,3,4,1,6,3,4,23])
#
# for a in arr:
#     for b in arr:
#         if a < b:
#             break
#     else:
#         print(a)
########################################################################################################################
# from numpy import*
# darr = array([
#     [1,2,3,4],
#     [2,3,4,5]
# ])
# darr3 = ([1,2,3,4,5,6,7])
# print(darr.ndim)  # Gives no of dimension of the array
# print(darr.shape)  # Gives no of rows and columns
# print(darr.size)  # Gives total number of elements
# darr1 = darr.flatten()  # Converts darr into 1d array
# print(darr1)
# darr2 = concatenate((darr3, darr1)) # mixes both arrays
# print(darr2)
########################################################################################################################
# Functions
# def prime_numbers_between(x,y):
#     k = 0
#     for i in range(x,y+1):
#         for a in range(2,i):
#             if i % a == 0:
#                 break
#         else:
#             print(i)
#             k+=1
#     print("There are", k, "Prime Numbers between", x, "and", y)
# prime_numbers_between(100,200)
########################################################################################################################
# def update(x):
#     print(x,id(x))
#     x = 10
#     print(x, id(x))
#
# a = 1
# print(a,id(a))
# update(a)
# print(a,id(a))
# # Therefore its neither pass by value nor pass by reference it will have same reference until value is changed and
# # reference is changed when value changes
########################################################################################################################
# def nameage(name = "Please enter your name",age= 18):
#     print(name)
#     if age < 18 or age > 110:
#         print("Please enter a valid age")
#     else:
#         print(age)
#
# nameage(name = "nk",age = 10000)
########################################################################################################################
# # variable length argument
# def sum(*b):
#     i = 0
#     for a in b:
#         i += a
#     print(i)
# sum(1,2,3)
# # keyword variable length argument
# def data(**data):
#     print(data)
# data(name = "nk", age = 16, phn = 9500000040)
########################################################################################################################
# # globals
# a = 1
# print(a, id(a))
# def fun():
#     globals()["a"] = 123
# print(a, id(a))
# fun()
########################################################################################################################
# def evod(list):
#     even = 0
#     odd = 0
#     for a in list:
#         if a % 2 == 0:
#             even += 1
#         else:
#             odd += 1
#     print("even", even)
#     print("odd", odd)
#
# list = []
# n = int(input("How many numbers are there to cheak"))
# y = int(input("Enter the first number"))
# for i in range(n-1):
#     x = int(input("Enter the next number"))
#     list.append(x)
# evod(list)
########################################################################################################################
# # Fibonacci numbers
# def fib(n,lessthan):
#     l = [0,1]
#     for i in range(n-2):
#         x = l[i+1]+l[i]
#         l.append(x)
#     print(l)
#     if l[n-1] <= lessthan:
#         print(l[n-1])
#     else:
#         for k in range(len(l)):
#             if l[k] > lessthan:
#                 break
#         print(l[k-1])
# fib(20,4181)
########################################################################################################################
# # Factorial of a number
# def factorial(n):
#     x = 1
#     for i in range(1,n+1):
#         x *= i
#     print(x)
# factorial(5)
########################################################################################################################
# # Fibonacci numbers
# n = int(input("How many fibonacci numbers do you want"))
# l = [0, 1]
# for i in range(n-2):
#     x = l[i+1]+l[i]
#     l.append(x)
# print(l)
########################################################################################################################
# # Recursion and limit in functions
# import sys
# sys.setrecursionlimit(2000)
# print(sys.getrecursionlimit())
# i = 0
# def recursion():
#     global i
#     print("Hello",i)
#     i += 1
#     recursion()
# recursion()
########################################################################################################################
# # Factorial using recursion
# def factorial(n):
#     if n == 0:
#         return 1
#     return n * factorial(n-1)
# print(factorial(5))
########################################################################################################################
# # Practice
# def factorial(k):
#     def fun(n):
#         if n==0:
#             return 1
#         else:
#             return n * fun(n-1)
#     print(fun(k))
#
# factorial(5)
########################################################################################################################
# # lambda function i.e., anonymous function
# f = lambda a,b : a+b
# print(f(2153,1234))
# # Using lambda
# ls = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
# print(list(filter(lambda n: n % 2, ls)))
# lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
# v = list(filter(lambda n: n % 2 == 0, lst))
# print(v)
# d = list(map(lambda n : n*2,v))
# print(d)
# from functools import reduce
# s = reduce(lambda a,b: a+b,d)
# print(s)
########################################################################################################################
# Decorators
# def div(a,b):
#     print(a/b)
#
# def smart_div(fun):
#     def inner(a,b):
#         if a<b:
#             a,b = b,a
#         return fun(a,b)
#     return inner
# div = smart_div(div)
#
# div(321,123)
########################################################################################################################
# v = int(input("Enter the number"))
# for i in range(100):
#     if 2**i > v:
#         print(i, "From", "         ",  -2**i, "To", 2**i,(i+1), "bit")
#         break
# bit = int(input("bit"))
# print(-2**(bit-1), "to", 2**(bit-1)-1)
########################################################################################################################
# def div(a,b):
#     print(a/b)
#
# def decor_div(func) :
#     def swaper(a,b):
#         if a < b:
#             a,b = b,a
#         return func(a,b)
#     return swaper
# div = decor_div(div)
# div(3,3)
########################################################################################################################
# from functions import *
# fibonacci(10)
# Prime_between(100,1000)
# factorial(10)
# print("My module is", __name__)
# ######################################################################################################################
# # OOPS = OBJECT ORIENTED PROGRAMMING
# class Computer:
#     def processor(self):
#         print("i9")
#     def ram(self):
#         print("16GB")
#     def rom(self):
#         print("1TB")
# c1 = Computer
########################################################################################################################
# class PC:
#     def __init__(self,cpu,ram):
#         print("Welcome")
#         self.cpu = cpu
#         self.ram = ram
#     def config(self):
#         print('config is', self.cpu, self.ram)
#
# com1 = PC('i5', '8gb')
# com2 = PC('i9', '32gb')
# print(1)
# com2.config()
# print(2)
# PC.config(com1)
########################################################################################################################
# class computer:
#     def __init__(self, age, name):
#          self.age = age
#          self.name = name
#
#     def compare(self,other):
#             if self.age == other.age:
#                 return True
#             else:
#                 return False
#
# C1 = computer(18, "nk")
# c1 = computer(23, "gk")
# I1 = id(C1)
# i1 = id(c1)
# if C1.compare(c1):
#     print("They are same")
# else:
#     print("THey are different")
# print(I1, i1)
########################################################################################################################
# # Instant and Class variable
# class jb_songs:
#     singer = "Justin Bieber"
#     def __init__(self, language, year_published):
#         self.lng = language
#         self.yrp = year_published
# baby = jb_songs("English", 2002)
# holy = jb_songs(year_published=2020, language="English")
# print(jb_songs.singer)
# print("Holy published in the year", holy.yrp)
# print("Baby is written in", baby.lng, "language")
# print("Holy is written in", holy.lng, "language")
# print("Baby published in the year", baby.yrp)
########################################################################################################################
# # Inheritance of class
# class A:
#     def __init__(self):
#         print("init A")
#     def feature(self):
#         print("Feature A")
#     def feature1(self):
#         print("Feature 1 is working")
#     def feature2(self):
#         print("Feature 2 is working")
# class B(A):
#     def __init__(self):
#         super().__init__()
#         print("init B")
#     def feature3(self):
#         print("Feature 3 is working")
#     def feature4(self):
#         print("Feature 4 is working")
# class C(B):
#     def __init__(self):
#         super().__init__()
#         print("init C")
#     def feature5(self):
#         print("Feature 5 is working")
#     def feature6(self):
#         print("Feature 6 is working")
# class D:
#     def __init__(self):
#         print("init D")
#     def feature(self):
#         print("Feature D")
#     def feature7(self):
#         print("Feature 7 is working")
#     def feature8(self):
#         print("Feature 8 is working")
# class E(A,D):                    # Method resolution order --> A,D
#     def __init_(self):
#         super().__init__()       # Hence it initiates 1st super class function i.e., in this case "A"
#         print("init E")
#     def feature9(self):
#         print("Feature 9 is working")
# o1 = A()
# o1.feature()
# o1.feature1()
# o1.feature2()
#
# o2 = B()
# o2.feature1()
# o2.feature2()
#
# o2.feature3()
# o2.feature4()
#
#
# o3 = C()
# o3.feature5()
# o3.feature6()
#
# o3.feature1()
# o3.feature2()
#
# o3.feature3()
# o3.feature4()
#
#
#
# o4 = D()
# o4.feature()
# o4.feature7()
# o4.feature8()

#
# o5 = E()
# o5.feature()                     # Ii takes function from first class in the order hence prints Feature A
# o5.feature9()
#
# o5.feature1()
# o5.feature2()
#
# o5.feature7()
# o5.feature8()


########################################################################################################################
# def div(a,b):
#     print(a/b)
#
# def smart_div(fun):
#     def inner(a,b):
#         if a<b:
#             a,b = b,a
#         return fun(a,b)
#     return inner
# div = smart_div(div)
#
# div(321,123)
# # Revision decorators
#
# def fun_sub(x,y):
#     print(x-y)
#
# def dec_sub(fun):
#     # fun_sub
#     def swap(a,b):
#         if a<b:
#             a,b = b,a
#             return fun(a,b)
#         else:
#             return fun(a,b)
#     return swap
# fun_sub = dec_sub(fun_sub)
#
# fun_sub(2,1)
########################################################################################################################
# DUCK TYPING EXAMPLES
# class apsara:
#     def writes(self):
#         print("Writes well")
# class natraj:
#     def writes(self):
#         print("Writes ruff")
# class book:
#     def text(self,pencil):
#         pencil.writes()
# pencil = natraj()
# b1 = book()
# b1.text(pencil)
####____________________________________________________________________________________________________________________
# class PyCharm:
#     def execute(self):
#         print("asdf")
#         print("sdfg")
# class Laptop:
#     def code(self,ide):
#         ide.execute()
#
# ide = PyCharm()
#
# lap1 = Laptop()
# lap1.code(ide)
#
# class class1:
#     def method(self):
#         print("Working")
# class executer:
#     def exe(self,obj):
#         obj.method()
#
#
# c1 = class1()
# exec = executer()
# exec.exe(c1)
########################################################################################################################
# # Iterators
# ls = [1,2,3,4,5,6]
# it = iter(ls)
# for i in range(len(ls)):
#     print(it.__next__())
#   # print(next(it))
# class number10:
#     def __init__(self):
#         self.number = 1
#     def __iter__(self):
#         return self
#     def __next__(self):
#         if self.number<=10:
#             vals = self.number
#             self.number += 1
#             return vals
#         else:
#             raise StopIteration
#
# num = number10()
# for i in num:
#     print(i)
########################################################################################################################
# class square10:
#      def __init__(self):
#          self.num = 1
#      def __iter__(self):
#          return self
#      def __next__(self):
#          if self.num <=10:
#              val = self.num**2
#              return val
#          else:
#              raise StopIteration
#
#
# # Generator(yield)
# class haf:
#     def __init__(self,div):
#         self.num = self
#
#     def div(self, div=2):
#         yield 5
#         yield 6
#         yield 7

# s = haf(123124)
# print(haf.div(s).__next__())
# print(haf.div(s).__next__())
# print(haf.div(s).__next__())

# def div(self,div = 2):
#     yield 5
#     yield 6
#     yield 7
# a = div(2,3)
# print(a.__next__())
# print(a.__next__())
# print(a.__next__())
# try:
#     x = float(input("Enter a number"))
#     print(x)
#     y = float(input("Enter a number"))
#     print(y)
#     print(x/y)
# except ValueError as t:
#     print("|Please enter a number not any other charachter|",t)
#     print("Task incomplete")
# except ZeroDivisionError as z:
#     print("Cant divide a number by ZERO")
#     print("Task incomplete")
# except Exception:
#     print("something went wrong")
#     print("Task incomplete")
# finally:
#     print("Bye")
########################################################################################################################
# from time import *
# from threading import *
# class Hello(Thread):
#     def run(self):
#         for i in range(10):
#             print("Hello")
#             sleep(0.1)
# class Hi(Thread):
#     def run(self):
#         for i in range(10):
#             print("Hi")
#             sleep(0.1)
# t1 = Hello()
# t2 = Hi()
# t1.start()  # Initiates thread 1(use getName to know name)
# sleep(0.05)
# t2.start()  # Initiates thread 1(use getName to know name)
# t1.join()  # Stops next commands
# t2.join()  # Stops next commands
# print("bye")  # By default initiated by the main thread
########################################################################################################################
# # Files
# rd = open("My file",'r')   # opens a file named "My file" if existed
# print(rd.read())   # gets the content of the file
# rdb = open("My file", 'rb')   # opens a file named "My file" if existed in binary format
# print(rdb.read())   # gets the content of the file in binary format
# wr = open("My file",'w')   # creates a file with name (My file) if not exists and u can write in it
# print(wr.write("Hello world"))   # write "Hello world" in the file
# wrb = open("My file", 'wb')   # creates a file with name(My file) if not exists and u can write in it in binary format
# # also cheakout open("My file",'a') which means appends the file etc
########################################################################################################################
# position = -1
# def search(list,value):
#     for i in range(len(list)):
#         if value == list[i]:
#             globals()['position'] = i+1
#             return True
#     return False
#
# ls = [1,2,3,4,5,6]
# n = int(input("Enter a value to search"))
# if search(ls,n):
#     print("Value found at", position)
# else:
#     print("Value not found")
########################################################################################################################
# # #   MY FIRST CODE EXPERIMENT
# # #   MEASURES OF CENTRAL TENDENCY
# # Taking input from user
# x = int(input("Enter number of values to check"))
# l = []
# for i in range(x):
#     y = float(input("Enter the next value"))
#     if y % 1 >= 0.5:
#         y = int(y) + 1
#     else:
#         y = int(y)
#
#     l.append(y)
# print("Given list of numbers is ", l)
# print("Here are the measures of central tendency for the list ")
# # Finding range and creating dummy frequency
# highest_number = 0
# least_number = 0
# for i in l:
#     for j in l:
#         if i<j:
#             break
#     else:
#         highest_number = i
# for i in l:
#     for j in l:
#         if i>j:
#             break
#     else:
#         least_number = i
# rng = highest_number - least_number + 1
# print("Least number", least_number)
# print("Highest number", highest_number)
# frequency = []
# for r in range(rng):
#     frequency.append(0)
# # print("Frequency", frequency)
# # Finding frequency values
# for frequency_index in range(len(frequency)):
#     for list_index in range(len(l)):
#         if l[list_index] == frequency_index+least_number:
#             frequency[frequency_index] += 1
# # print("Frequency", frequency)
# highest_frequency = 0
# for i in frequency:
#     for j in frequency:
#         if i<j:
#             break
#     else:
#         highest_frequency = i
# print(highest_frequency)
# # Calculating Median
# median = 0
# lm = l.copy()
# a_o_list = []
# for q in range(len(lm)):
#     for a in lm:
#         for b in lm:
#             if a > b:
#                 break
#         else:
#             a_o_list.append(a)
#             lm.remove(a)
# print("Ascending order of the list is", a_o_list)
# # Calculating different types of means
# arithmetic_mean = 0
# for i in range(len(l)):
#     arithmetic_mean += l[i]
# arithmetic_mean /= len(l)
# print("Arithmetic mean is", arithmetic_mean)
# geometric_mean = 1
# for i in range(len(l)):
#     geometric_mean *= l[i]
# geometric_mean = geometric_mean**(1/len(l))
# print("Geometric mean is", geometric_mean)
# harmonic_mean = 0
# for i in range(len(l)):
#     harmonic_mean += 1/l[i]
# harmonic_mean = len(l)/harmonic_mean
# print("Harmonic mean is", harmonic_mean)
#
# if len(a_o_list)%2 == 0:
#     median = (a_o_list[int((len(a_o_list))/2)]+a_o_list[int((len(a_o_list))/2) - 1])/2
# else:
#     median = a_o_list[int(((len(a_o_list))-1)/2)]
# print("Median is", median)
# # Printing Mode
# if highest_frequency == 1:
#     print("There is NO MODE since no number is repeated")
# else:
#     number_of_modes = 0
#     for i in range(len(frequency)):
#         if int(frequency[i]) == int(highest_frequency):
#             number_of_modes += 1
#     if number_of_modes >1:
#         print("There are ", number_of_modes, "Modes for this list. They are ", end="")
#         for i in range(len(frequency)):
#             if int(frequency[i]) == int(highest_frequency):
#                 print(i+least_number, end=", ")
#         print("and they are repeated", highest_frequency, "times each")
#     else:
#         for i in range(len(frequency)):
#             if int(frequency[i]) == int(highest_frequency):
#                 print("Mode is ", i+least_number, "and it is repeated", highest_frequency, "times")
#
# print("Range of the given values is", highest_number - least_number)
########################################################################################################################
# lst = []
# for i in range(1000):
#     lst.append(i)
# search = 501
# low_bound = 0
# high_bound = int(len(lst))
# for i in range(len(lst)):
#     if search == low_bound:
#         print(search, "Found at ", low_bound)
#         break
#     elif search == high_bound:
#         print(search, "Found at", high_bound)
#         break
#     elif search < lst[(high_bound+low_bound)//2]:
#         high_bound = (high_bound+low_bound)//2
#     elif search > lst[(high_bound+low_bound)//2]:
#         low_bound = (high_bound+low_bound)//2
#     elif search == lst[(high_bound+low_bound)//2]:
#         print(search, "Found at", lst[(high_bound+low_bound)//2])
#         break
#     else:
#         pass
#
#
# else:
#     print("Not found")
########################################################################################################################
# l1 = [-1, 3, 8, 9, 5]
# l2 = [4, 1, 2, 10, 5, 20]
# t = 24
# lt = []
# x = 0
# for i in l1:
#     for j in l2:
#         if i+j < t:
#             lt.append(t-(i+j))
#         else:
#             lt.append(i+j-t)
# for i in range(len(lt)):
#     for j in range(len(lt)):
#         if lt[i] > lt[j]:
#             break
#     else:
#         x = lt[i]
# # print(x)
# for i in l1:
#     for j in l2:
#         if i+j - t == x or t - (i+j) == x:
#             print(i, " form l1 and ", j, "from l2")

########################################################################################################################
