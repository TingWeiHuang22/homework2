# homework2

**電腦視覺特效-第六組**  
  
## Training  
  
* 在這次作業training的時候，我們這組所選擇的dataset為summer2winter_yosemite此組dataset，而在training的過程中，我們組員原本認為training 一百萬個iterations大概只要花費兩天的時間，而在training到整整三天後，發現iterations只有跑到五十七萬。因為時間不足的因素，所以我們model只有training 到五十七萬iterations。(附圖是我們這次training過程中所顯示的資訊)  
  
![alt text](pictures/training/training1.png)  
  
* 以下附圖是training的過程中，每10000 iterations會儲存的checkpoints pt檔案(含有discriminator 以及 generator)
  
![alt text](pictures/training/training2.png)
  
* 以下training過程中，各個iterations(分別為1萬 10萬 20萬 30萬 40萬 50萬 57萬)在A to B(summer to winter) 結果照片顯示。每張照片的第一列為圖片原本的content，而在第二列至第五列分別為原本圖片換上有winter style的結果圖，而由以下圖片可以得知，training iterations的多寡，在某些圖片上面並不能證明iterations越多，style transfer效果會越好。
  
![alt text](pictures/training/training3.png)  
![alt text](pictures/training/training4.png)  
![alt text](pictures/training/training5.png)  
![alt text](pictures/training/training6.png)  
![alt text](pictures/training/training7.png)  
![alt text](pictures/training/training8.png)  
![alt text](pictures/training/training9.png)

## Inference
  
**content**\\**style** 
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer2.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer5.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer7.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer8.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/9.jpg" width="100" height="100"/>
<br/>
  
    
## Compare with other method  



  
  
  


