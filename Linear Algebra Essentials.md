# Linear Algebra: The Robin of Dataman
#### by Yue Chen

Linear algebra is a branch of mathematics that is extremely useful in data science. It is also the most important math skill in machine learning, as most machine learning models can be expressed in matrix form, like how a dataset itself is often represented as a matrix. Not only has been used in data preprocessing, data transformation, and model evaluation, under the hood, linear algebra powers major areas including the cutting-edge fields of Natural Language Processing and Computer Vision. Hence, we can say that, if Data Science was Batman, Linear Algebra would be Robin. Here are the topics you need to be familiar with:

## 1.	Vector
To help you better understand the concept and features of vector, let’s start with a comparative study of Scalar VS Vector.

Scalar Definition: A scalar is a number. Examples of scalars are temperature, distance, speed, or mass – all quantities that have a magnitude but no “direction”, other than perhaps positive or negative.   
<img src="LA_Images/p1.png" width="400" height="250">

Vector Definition: A vector is a list of numbers. There are (at least) two ways to interpret what this list of numbers mean: 1. Think of the vector as being a point in a space. Then this list of numbers is a way of identifying that point in space, where each number represents the vector’s component that dimension. Or 2. Think of a vector as a magnitude and a direction, e.g. a quantity like velocity. In this way of think of it, a vector is a directed arrow pointing from the origin to the end point given by the list of numbers.  
 <img src="LA_Images/p2.png" width="400" height="300">

## 2.	Matrix

 <img src="LA_Images/p3.gif" width="500" height="200">
 
Again, speaking of matrix, the introduction of determinant is inevitable. 

Definition: Both determinants and matrices are logical and convenient representations of large sets of real numbers or variables and vectors, which are arranged in arrays of rows and columns.

Differences:
1.	a matrix is a group of numbers but a determinant is a unique number related to that matrix. 

2.	In writing, we distinguish them by using two brackets to cover numbers in matrix, while using tow bars to covered numbers in determinant.

3.	In a matrix: the number of rows doesn’t need to be equal to the number of columns;
In a determinant: the number of rows === the number of columns.

 <img src="LA_Images/p4.png" width="220" height="320">

## 3. Properties of matrix

3.1 Transpose of a matrix:
Definition: The transpose of an m x n matrix A is the n x m matrix AT obtained by interchanging rows and columns of A.

 <img src="LA_Images/p5.png" width="550" height="170">

Try transposing a matrix using your right hand (following this paw):

 <img src="LA_Images/p6.png" width="500" height="210">
                             
3.2 Inverse of a matrix
The inverse of matrix is another matrix, which on multiplication with the given matrix gives the multiplicative identity. For a matrix A, its inverse is A-1, and A.A-1 = A-1·A = I, where I is the identity matrix.
          
 <img src="LA_Images/p7.png" width="400" height="220">    <img src="LA_Images/p8.png" width="237" height="200">

## 4.	Dot product and matrix multiplication

Definition: The dot product is an algebraic operation that takes two same-sized vectors and returns a single number.

<img src="LA_Images/p9.png" width="600" height="120">
                                 
Geometric definition: the dot product is the product of the Euclidean magnitudes of two vectors and the cosine of the angle between two.

<img src="LA_Images/p10.png" width="600" height="230">

Definition of Matrix multiplication: basically, a matrix version of the dot product. Remember the result of dot product is a scalar. The result of matrix multiplication is a matrix, whose elements are the dot products of pairs of vectors in each matrix. 

<img src="LA_Images/p11.png" width="485" height="230">


Requirement: 
 the 1st matrix must have the same number of columns as the 2nd matrix has rows.

## 5. Eigenvalues and Eigenvectors

Definition:
Eigenvector: Every vector (list of numbers) has a direction when it is plotted on XY chart. Eigenvectors are those vectors when a linear transformation (such as multiplying it to a scalar) is performed on them, their direction does not change.
Eigenvalue: The scalar that is used to transform (stretch/compress) an Eigenvector.
 
<img src="LA_Images/eigen1.png" width="275" height="109">

In matrix form

<img src="LA_Images/eigen2.png" width="1000" height="360">

Meaning: 

Eigenvalues and Eigenvectors provides summary of a large matrix.
Eigenvectors and eigenvalues are used to reduce noise in data. They can help us improve efficiency in computationally intensive tasks. They also eliminate features that have a strong correlation between them and also help in reducing over-fitting. The core of component analysis (PCA) is built on the concept of eigenvalues and eigenvectors. Additionally, eigenvectors and eigenvalues are used in facial recognition techniques such as EigenFaces.

Lastly, in non-linear motion dynamics, eigenvalues and eigenvectors can be used to help us understand the data better as they can be used to transform and represent data into manageable sets.

## References

Matrix: 
https://www.mathsisfun.com/search/search.html?query=linear+algebra&submit=&search=1#ff

Eigenvalues and Eigenvectors: 
https://medium.com/sho-jp/linear-algebra-part-6-eigenvalues-and-eigenvectors-35365dc4365a

