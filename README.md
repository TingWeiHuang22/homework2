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
* 以下表格為使用MUNIT跑personal image的結果(first row為各個style的圖片，first column為各個content的圖片，而表格的其他圖片為inference的結果)
  
**content**\\**style**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/9.jpg" width="100" height="100"/>
<br/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer1.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/1/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer2.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/2/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer3.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/3/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer4.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/4/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer5.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/5/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer6.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/6/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer7.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/7/9.jpg" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer8.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/inference/8/9.jpg" width="100" height="100"/>
<br/>
  
    
## Compare with other method  
* 以下表格為使用FasterPhotoStyle跑相同的personal image的結果(first row為各個style的圖片，first column為各個content的圖片，而表格的其他圖片為FasterPhotoStyle方法所inference的結果)
    
**content**\\**style**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/1.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/3.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/4.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/6.jpg" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_style/9.jpg" width="100" height="100"/>
<br/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer1.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/1/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/1/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/1/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/1/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/1/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer2.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/2/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/2/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/2/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/2/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/2/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer3.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/3/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/3/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/3/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/3/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/3/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer4.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/4/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/4/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/4/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/4/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/4/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer5.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/5/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/5/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/5/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/5/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/5/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer6.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/6/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/6/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/6/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/6/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/6/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer7.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/7/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/7/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/7/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/7/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/7/9.png" width="100" height="100"/>
<br/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/input_content/summer8.jpg" width="100" height="100"/>
&nbsp;&nbsp;&nbsp;
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/8/1.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/8/3.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/8/4.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/8/6.png" width="100" height="100"/>
<img src="https://github.com/TingWeiHuang22/homework2/blob/master/pictures/FastPhotoStyle/8/9.png" width="100" height="100"/>
<br/>
  
  
* 在上述MUNIT的表格所inference的效果，可以發現style的效果有很貼切的改變了content的內容，且Inference的成果我認為是有改變原本圖片的style成另外一種風韻的圖片。而吾人認為效果最好的是forth row的各個inference結果，因為它會讓人真心認為這些圖片是由畫家畫出而非合成的結果。
* 然而在FasterPhotoStyle的表格所inference的效果，可以發現style的效果雖然有影響原本圖片的content，然而卻會讓人覺得inference過頭的感覺，特別是某些inference的結果是整個照片糊掉而無法呈現原本圖片中的場景的內容。
* 綜合上述所言，吾人認為MUNIT所Inference的結果，會比FasterPhotoStyle所Inference的結果還要好。雖然在FasterPhotoStyle的github中，透過FasterPhotoStyle所inference的結果也相當令人驚豔，但是吾人認為就目前測試結果整體性而言，MUNIT所呈現的Inference效果是比FasterPhotoStyle更robust的。


  
  
  


