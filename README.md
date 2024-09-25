# ways-to-make-a-array

ndarray object attributes
======================================================================
=>here ndarray object contains the following Attributes

1. dtype
2. ndim
3. shape
4. size
5. itemsize

				objectofndarray.attribute name

   
->They are 17 ways to make an nd.array
=>We know that ndarray is one of the pre-defined class present in numpy module.
=>The object of ndarray is used for Storing the Data in the form 1-D, 2-D and N-D arrays.
=>To create an object of ndarray, we have Many Approaches.

			1. array()
			2. arange()
			3. zeros()
			4. ones()
			5. full()
			6. linspace()
			7. eye()
			8. identity()
			9. hstack()
			10.vstack()
			-------------------------------------
			numpy.random
			-------------------------------------
				11. randint()
				12. randn()
				13. normal()
				14. rand()
				15. uniform()
				16. choice()
				17. shuffle()


2. arange()
==========================================================
=>Syntax:      varname=numpy.arange(Value)---->Gives Range of Values from 0 to Value-1---ndarray---1-D

=>Syntax:      varname=numpy.arange(Start,Stop)---Gives Range of values from Start to stop-1--ndarray--1D

 >Syntax:      varname=numpy.arange(Start,Stop,Step)--Gives Range of values from Start to stop-1 by maintaining 
								Equal Interval of Step either in Forward Direction or in Backward direction-----ndarray------1D
=>here arange() cerated -1D of ndarray object But not able to create 2-D and n-D Objects.
=>To create  2-D and n-D Objects of ndarray, we must use shape attribute or reshape()
-----------------------------------------------------------------------------------------------------------------------------
3. zeros():

Syntax:	varname=numpy.zeros(shape,dtype)
=>This function is used for Bulding ndarray object by initlizing all the entries as 0
=>Here shape Represents 1-D (No of Zeros), 2-D (Row x Cols ) and 3-D (No. of Matrices, Rows , Cols )

-----------------------------------------------------------------------------------------------------------------------------
4. linspace()
===============================================================================================
Syntax:     varname = numpy.linspace(start, stop, num, endpoint, retstep, dtype)   
=>start: It represents the starting value of the interval.
=>stop:It represents the stopping value of the interval.
=>num: The amount of evenly spaced samples over the interval to be generated. The default is 50.
=>endpoint: Its true value indicates that the stopping value is included in the interval.
=>rettstep: This has to be a boolean value. Represents the steps and samples between the consecutive numbers.
=>dtype: It represents the data type of the array items.
===============================================================================================					
5. ones():
   
=>This Function is used for building ONEs matrix either with 1-D or 2-D or n-D 
=>Syntax:   varname=numpy.ones(shape,dtype)

>Here Shape can be 1-D(number of ones)  or 2-D(Rows,Cols)  or n-D( Number of Matrices,Number of Rows, Number of Columns) 
===============================================================================================
6.  full():

=>This is function is used for building a matrix by specifying fill value either 1-D or 2-D or n-D
=>Syntax:-
			varname=numpy.full(shape,fill_value,dtype)
=>varname is an obejct of <class, numpy.ndarray>
=>Here Shape can be 1-D(number of  Fill_Value)  or 2-D(Rows,Cols)  or n-D( Number of Matrices,Number of Rows, Number of Columns) 
=>fill_value can be any number of programmer choice 

===============================================================================================
7.  identity():

=>This function always bulid Identity or unit matrix 
=>Syntax:-  varname=numpy.identity(N,dtype)
=>Here N represents Either we can take Rows or Columns and PVM takes as NXN Matrix (Square Matrix--Unit or Identity)

==================================================================================================
 8.eye():
 
=>The eye() function is used to create a 2-D array with ones on the diagonal and zeros elsewhere.
=>The eye() function is commonly used in linear algebra and matrix operations. It is useful for generating matrices to transform, rotate, or scale vectors. It can also be used in scientific computing for solving differential equations, optimization, and signal processing.
-------------------------
Syntax:   numpy.eye(N, M=None, k=0, dtype)
-------------------------
N---->Number of rows in the output.	Required
M--->Number of columns in the output. If None, defaults to N.	
k--->	Index of the diagonal: 0 (the default) refers to the main diagonal, a positive value refers to an upper diagonal, and		a negative value to a lower diagonal.	
dtype--->Data-type of the returned array.	

===============================================================================================
  9.hstack()

		varname=numpy.hstack((ndarrayobj1,ndarrayobj2))

=>The function nnumpy.hstack(tup) takes arguments as tuple which include matrix's/arrays. The hstack function combines the two or more matrix/arrays horizontally which have the same number of rows. The hstack returns an ndarray.

===============================================================================================
  10.vstack()

		varname=numpy.vstack((ndarrayobj1,ndarrayobj2))
=>The function nnumpy.vstack(tup) takes arguments as tuple which include matrix's/arrays. The vstack function combines the two or more matrix/arrays Verticaly which have the same number of Columns. The vstack returns an ndarray.
