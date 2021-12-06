# HPC Laboratory Work №4: Salt and Pepper
# Assignment
Given the image of size M×N with "Salt and Pepper" noise, implement and apply a CUDA version of 9-point
median filter and store the result to output image. Missing values for edge rows and columns are to be taken from
nearest pixels.


# Tools<br>
Programming language: Python v3.7.12<br>
IDE: Google Colaboratory<br>
GPU: Tesla K80<br>
CPU: Intel(R) Xeon(R) CPU @ 2.30GHz

# Experiments

## Image 1
This image has 91908 elements
|Original Image | Salt and Paper | CPU filtering | GPU filtering | 
|:----:|:----:|:----:|:----:|
|![Screenshot](images/price1.jpg) | ![Screenshot](images/SAP1.jpg) | ![Screenshot](images/CPU1.jpg) | ![Screenshot](images/GPU1.jpg) | 
| --- | --- | 1.3400<br>seconds | 0.0008<br>seconds | 

## Image 2
This image has 172800 elements
|Original Image | Salt and Paper | CPU filtering | GPU filtering | 
|:----:|:----:|:----:|:----:|
|![Screenshot](images/price3.jpg) | ![Screenshot](images/SAP3.jpg) | ![Screenshot](images/CPU3.jpg) | ![Screenshot](images/GPU3.jpg) | 
| --- | --- | 2.3731<br>seconds | 0.0011<br>seconds | 

## Image 3
This image has 810000 elements
|Original Image | Salt and Paper | CPU filtering | GPU filtering | 
|:----:|:----:|:----:|:----:|
|![Screenshot](images/price2.jpg) | ![Screenshot](images/SAP2.jpg) | ![Screenshot](images/CPU2.jpg) | ![Screenshot](images/GPU2.jpg) | 
| --- | --- | 11.2826<br>seconds | 0.0032<br>seconds | 

## Image 4
This image has 1047552 elements
|Original Image | Salt and Paper | CPU filtering | GPU filtering | 
|:----:|:----:|:----:|:----:|
|![Screenshot](images/price4.jpg) | ![Screenshot](images/SAP4.jpg) | ![Screenshot](images/CPU4.jpg) | ![Screenshot](images/GPU4.jpg) | 
| --- | --- | 15.1601<br>seconds | 0.0037<br>seconds | 

## Image 5
This image has 2073600 elements
|Original Image | Salt and Paper | CPU filtering | GPU filtering | 
|:----:|:----:|:----:|:----:|
|![Screenshot](images/price5.jpg) | ![Screenshot](images/SAP5.jpg) | ![Screenshot](images/CPU5.jpg) | ![Screenshot](images/GPU5.jpg) | 
| --- | --- | 29.0027<br>seconds | 0.0072<br>seconds | <br><br>

# Results

| Original Image | CPU filtering | GPU filtering | Boost
|:----:|:----:|:----:| :----:|
| Image 1 | 1.3400<br>seconds | 0.0008<br>seconds | 1578.8294 |
| Image 2 | 2.3731<br>seconds | 0.0011<br>seconds | 2144.7138 |
| Image 3 | 11.2826<br>seconds | 0.0032<br>seconds | 3518.1529 |
| Image 4 | 15.1601<br>seconds | 0.0037<br>seconds | 3997.1175 |
| Image 5 | 29.0027<br>seconds | 0.0072<br>seconds | 4004.4172 |

# Conclusion
Based on the temporal performance of the algorithms, as well as the acceleration rate,<br>
it becomes obvious that the use of GPU for filtering is completely justified,<br>
especially in the case of an increased image resolution with a large number of elements in the image.
