---
layout: post
title: Check Symmetrical Days Using R
categories: [R language, symmetrical day, yyyymmdd]
tags: [fun]
comments: yes
---

I still clearly remembered in November 2nd, 2011, someone said we may never meet another symmetrical day in your lifetime, so please cherish this special day. The so-called symmetrical day means that in the date format which looks like "yyyymmdd", the first letter of the year is the last letter of the day, and the second letter of the year is the first letter of the day, and so on. Yes, these cases are rare, but I'd like to know the next symmetrical day afte "20111102". Does no more symmetrical day exist in the near future? Three years ago, I was a beginner in R language, so I try to write several lines of code to check how many symmetrical days are from year 2000 to 2999? 

Here is the code:

{% highlight r %}
a <- 2000:2999 ## all years
b <- c(paste("0",1:9,sep=""),10,11,12) ## the month
c <- c(paste("0",1:9,sep=""),10:31) ## the day
mmdd <- paste(rep(b,each=31),rep(c,time=12),sep="") ## 'mmdd'
all <- paste(rep(a,each=length(mmdd)),rep(mmdd,time=length(a)),sep="") ## all days formatted as 'yyyymmdd'
s12 <- substr(all,1,2) ## first two letters in 'yyyymmdd'
s34 <- substr(all,3,4) ## third and fourth letters in 'yyyymmdd'
s56 <- substr(all,5,6) ## fifth and sixth letters in 'yyyymmdd'
s78 <- substr(all,7,8) ## last two letter in 'yyyymmdd'
rev.s56 <- paste(substr(s56,2,2),substr(s56,1,1),sep="") ## reverse the order of these two letters
rev.s78 <- paste(substr(s78,2,2),substr(s78,1,1),sep="") ## reverse the order of these two letters
sym.day <- all[(s12==rev.s78)&(s34==rev.s56)] ## whether this day is symmetrical
sym.day
{% endhighlight %}

After running around a couple of seconds, the result comes out:

`> sym.day`

	[1] "20011002" "20100102" "20111102" "20200202" "20211202" 
	[6] "20300302" "20400402" "20500502" "20600602" "20700702"
	[11] "20800802" "20900902" "21011012" "21100112" "21111112"
	[16] "21200212" "21211212" "21300312" "21400412" "21500512"
	[21] "21600612" "21700712" "21800812" "21900912" "22011022"
	[26] "22100122" "22111122" "22200222" "22211222" "22300322"
	[31] "22400422" "22500522" "22600622" "22700722" "22800822"
	[36] "22900922"

The result shows we will meet the next symmetrical day in February 2nd, 2020, and totally have 36 symmetrical days from year 2000 to 2999. If you want to check the symmetrical days from year 3000 to 3999, just modify the first line of the code as `a <- 3000:3999`, and the result will pop up. With the help of R language, the problem was easily figured out. Although originally I wrote the code for fun, it was my first step to entry the world of R language three years ago.
