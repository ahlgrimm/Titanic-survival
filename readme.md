---
title: "Titanic survival"
author: "Marius Ahlgrimm"
date: "1 April 2019"
output:
  pdf_document: default
---





```
##      pclass         survived         name               sex           
##  Min.   :1.000   Min.   :0.000   Length:1309        Length:1309       
##  1st Qu.:2.000   1st Qu.:0.000   Class :character   Class :character  
##  Median :3.000   Median :0.000   Mode  :character   Mode  :character  
##  Mean   :2.295   Mean   :0.382                                        
##  3rd Qu.:3.000   3rd Qu.:1.000                                        
##  Max.   :3.000   Max.   :1.000                                        
##                                                                       
##       age              sibsp            parch          ticket         
##  Min.   : 0.1667   Min.   :0.0000   Min.   :0.000   Length:1309       
##  1st Qu.:21.0000   1st Qu.:0.0000   1st Qu.:0.000   Class :character  
##  Median :28.0000   Median :0.0000   Median :0.000   Mode  :character  
##  Mean   :29.8811   Mean   :0.4989   Mean   :0.385                     
##  3rd Qu.:39.0000   3rd Qu.:1.0000   3rd Qu.:0.000                     
##  Max.   :80.0000   Max.   :8.0000   Max.   :9.000                     
##  NA's   :263                                                          
##       fare            cabin             embarked        
##  Min.   :  0.000   Length:1309        Length:1309       
##  1st Qu.:  7.896   Class :character   Class :character  
##  Median : 14.454   Mode  :character   Mode  :character  
##  Mean   : 33.295                                        
##  3rd Qu.: 31.275                                        
##  Max.   :512.329                                        
##  NA's   :1                                              
##      boat                body        home.dest        
##  Length:1309        Min.   :  1.0   Length:1309       
##  Class :character   1st Qu.: 72.0   Class :character  
##  Mode  :character   Median :155.0   Mode  :character  
##                     Mean   :160.8                     
##                     3rd Qu.:256.0                     
##                     Max.   :328.0                     
##                     NA's   :1188
```


```
##      pclass    survived        name         sex         age       sibsp 
##           0           0           0           0         263           0 
##       parch      ticket        fare       cabin    embarked        boat 
##           0           0           1        1014           2         823 
##        body   home.dest       Title family_size 
##        1188         564           0           0
```

```
## ntree      OOB      1      2
##   300:  18.79% 11.12% 31.20%
## ntree      OOB      1      2
##   300:  18.95% 11.00% 31.80%
## ntree      OOB      1      2
##   300:  19.25% 11.00% 32.60%
## ntree      OOB      1      2
##   300:  19.33% 11.25% 32.40%
## ntree      OOB      1      2
##   300:  18.79% 11.37% 30.80%
```




![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-1.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-2.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-3.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-4.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-5.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-6.png)![plot of chunk unnamed-chunk-11](figure/unnamed-chunk-11-7.png)

![plot of chunk unnamed-chunk-12](figure/unnamed-chunk-12-1.png)

<table>
 <thead>
  <tr>
   <th style="text-align:left;">   </th>
   <th style="text-align:right;"> Linear </th>
   <th style="text-align:right;"> Polynomial </th>
   <th style="text-align:right;"> Radial </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Train </td>
   <td style="text-align:right;"> 0.2206304 </td>
   <td style="text-align:right;"> 0.1852913 </td>
   <td style="text-align:right;"> 0.1824260 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> CV </td>
   <td style="text-align:right;"> 0.2206868 </td>
   <td style="text-align:right;"> 0.1900733 </td>
   <td style="text-align:right;"> 0.1852381 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Test </td>
   <td style="text-align:right;"> 0.2175573 </td>
   <td style="text-align:right;"> 0.1832061 </td>
   <td style="text-align:right;"> 0.1832061 </td>
  </tr>
</tbody>
</table>

![plot of chunk unnamed-chunk-14](figure/unnamed-chunk-14-1.png)



![plot of chunk unnamed-chunk-16](figure/unnamed-chunk-16-1.png)


<table>
 <thead>
  <tr>
   <th style="text-align:left;">   </th>
   <th style="text-align:left;"> RF </th>
   <th style="text-align:right;"> SVM </th>
   <th style="text-align:right;"> KNN </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Train </td>
   <td style="text-align:left;"> 0.0811843 </td>
   <td style="text-align:right;"> 0.1824260 </td>
   <td style="text-align:right;"> 0.1977077 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> CV </td>
   <td style="text-align:left;">  </td>
   <td style="text-align:right;"> 0.1852381 </td>
   <td style="text-align:right;"> 0.3027569 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Test </td>
   <td style="text-align:left;"> 0.1641221 </td>
   <td style="text-align:right;"> 0.1832061 </td>
   <td style="text-align:right;"> 0.1832061 </td>
  </tr>
</tbody>
</table>






