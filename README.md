# code-training
C++ code training

1.vector
向量（Vector）是一个封装了动态大小数组的顺序容器（Sequence Container）。跟任意其它类型容器一样，它能够存放各种类型的对象。可以简单的认为，向量是一个能够存放任意类型的动态数组。

关于vector\<vector\<int\> \> A类型
  
  1、定义  
     vector\<vector\<int\> \> A;//正确的定义方式  
  2、插入元素  
     若想定义A = [[0,1,2],[3,4,5]]，则：  
     //正确的插入方式     
     vector\<vector\<int\> \> A;      
     //A.push_back里必须是vector         
     vector<int> B;       
     B.push_back(0);       
     B.push_back(1);       
     B.push_back(2);       
     A.push_back(B);       
     B.clear();       
     B.push_back(3);       
     B.push_back(4);      
     B.push_back(5);       
     A.push_back(B);  
