# BackMIC
A new method, BackMIC, to calculate the MIC values

Source code of the BackMIC

## 1） MATLAB is the tool of Chi-MIC;    
## 2)  Make sure that c++ has installed in your computer for compilation;  In the matlab runtime environment, use the ```mex -setup``` command to set: <use of'Microsoft Visual C++' for C++ language compilation>
## 3)  Running program “make.m” to compile the equipartitionYaxis2.c, getsuper2var.c and getmutualI2var_fix4.c to mex files;
> The first column of data is Y (dependent variable), the rest of the columns (X) independent variable;
    
    make;  
    num=randperm(size(data,1));   
    data=data(num',:);% scramble the samples  

## Y is numerical data
    sample_num=size(data,1); 
    [MIC,thebestc1,thebestc2]=MIC_OIC_chi_1_1_back(data,sample_num^0.55,5,sample_num)

    
    
Source: 
An improved algorithm for the maximal information coefficient and its application
## Contact me：chenyuan0510@126.com

