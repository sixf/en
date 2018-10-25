---
title: PeerJ：Next PLoS ONE？
layout: post
categories: [academic]
tags: [journal,ecology,public review,preprint,Open Access,Impact factor]
comments: yes
---

PLoS ONE, the academic publishing giant which was founded in  December 2006, publishs [more than ten thousands](http://en.wikipedia.org/wiki/PLOS_ONE) artices each year since 2011, and the number is still increasing dramatically. Published so many articels, PLoS ONE did earn a lot with the price of $1350 for each article. Due to its large number of the published articels, the quality of each article is inevitably uneven. As a result, many schloars and institutes have different opinions on PLoS ONE: someone consider PLoS ONE as a great journal, while othes disagree on that.

Now, we should pay attention to another newly founded Open Access journal--[PeerJ](http://peerj.com). PeerJ was co-founded by publisher Peter Binfield (formerly at PLoS ONE) and CEO Jason Hoyt (formerly at Mendeley as Chief Scientist) in June 2012. Although PeerJ is also an Open Access journal, it has completely different [business model](https://peerj.com/pricing/). PeerJ offers three membership plans: the basic plan ($99) allows researchers to publish one paper per year; an enhanced plan ($199) allows two paper annually, and the investigator plan ($299) allows to publish unlimited articles on PeerJ in the future. Comparing other Open Access journals, such as PLoS ONE, the publication fee of PeerJ is much cheaper. Whether this creative bussiness model will be successful or not, it needs more time to verify.

In April 2014, I submitted [a manuscript on the topic of camera traps](https://peerj.com/articles/374/) to PeerJ, which was finally accepted in one month after the date of my submission. Based on this experience, I here briefly share some opinions on what I think about PeerJ. I extracted the basic information of the first 365 articels ([download(43KB)](http://sixf.org/files/code/2014/05/peerj365.txt)) published by PeerJ from February 12, 2013 to April 22, 2014 using R language ([download the R code (3KB)](http://sixf.org/files/code/2014/05/peerj.txt)), including the received date, accepted date, published data, publish their review histories or not and the citation of each article. Based on the information, I made a simple analysis.

-	**Review speed**. I have to admit that the review process of PeerJ is very fast. As advertised by PeerJ, the medium time for the articels submitted from December 2012 to July 2013 which received their first decisions was [24 days](http://blog.peerj.com/post/60259877854/peerj-speed). I simply analyzed the receive time (the number of days from submission to acceptance) and publish time (the number of days from acceptance to online) for these 365 articles in 2013 and 2014, respectively, which were shown in the following table:

---

<table>
	<tbody>
		<tr>
			<td>Year </td>
			<td>No. of Articles</td>
			<td>Receive (Medium)</td>
			<td>Receive (Mean±SD)</td>
			<td>Publish (Medium)</td>
			<td>Publish (Mean±SD)</td>
		</tr>
		<tr>
			<td>2013</td>
			<td>232</td>
			<td>56</td>
			<td>69 ± 46</td>
			<td>23</td>
			<td>26 ± 11</td>
		</tr>
		<tr>
			<td>2014</td>
			<td>133</td>
			<td>71</td>
			<td>81 ± 53</td>
			<td>28</td>
			<td>29 ± 11</td>
		</tr>
		<tr>
			<td>Total</td>
			<td>365</td>
			<td>60</td>
			<td>73 ± 49</td>
			<td>24</td>
			<td>27 ± 11</td>
		</tr>
	</tbody>
</table>

---


-	**Publish review history**. I believe this is another improvement besides [the lower publication fee](http://blog.peerj.com/post/66773028124/peerj-saves-academia-money), comparing PLoS ONE. As [introduced](http://blog.peerj.com/post/58170809555/peerj-six-month-review) by PeerJ on its official website, more than 80% of the authors chose to [set their review history as public](https://peerj.com/reviews/), which means all the documents relating to the original submission, revision, editor and reviewers' comments and the rebutter letter are freely avaliable to download. I analyzed the data of review history extracted from PeerJ website of these 365 articles: for all articles, 77% of authors published the review history of their articles, and 75% in 2013, 81% in 2014, with a trend that more authors will like to publish their review histories in the future. Of course, all the academic editors are not confiendital, and nearby [43%](http://blog.peerj.com/post/58170809555/peerj-six-month-review) of reviewers chose to set their names as public. Here I must note that, such as a junior researcher as myself, these public review histories provide numerous learning materials to educate me how to reply the reviewers' or editors' comments! 
-	**Editor group**. In reality, the prestige of a journal mostly depends on the team of editors. Currently, PeerJ has [845 editors](https://peerj.com/academic-boards/editors/), which is a world-leading group, including some Nobel Prize winners. I have a special interest that, to date, PeerJ only published around 370 articles, indicating that most of editors did not handle any manuscript. Therefore, I analyzed the editors of these 365 articles, and found that totally there were 190 editors, approxemately 22% of editors in the editorial board of PeerJ. It seems like that nearly 78% of editors did not contribute editorial services (they might edit the manuscripts that were finally rejected), but some editors had already edited several articles. For exmaple, one editor had handled [17 published articles](https://peerj.com/JafriMAbdullah/). 80% of editors (152/190) had edited one manucript, which shown as the following figure ([download (3KB)](http://sixf.org/files/code/2014/05/editors.txt) this full list)：

![](http://sixf.org/files/images/2014/05/peerj_editors.png)

-	**Impact factor**. Because PeerJ began to publish articles officially since 2013, it still has [no impact factor](http://blog.peerj.com/post/81475988271/announcing-new-data-reports-for-peerj-articles). However, we might have a glimpse for the 365 articles from these exsiting citation records. Here, to calcualte the *impact factor* conservely, I used the citations on PeerJ website, rather than the data from Google Scholar, becasue Google Scholar indexed more journals which are not SCI journals. The results showed that, as of May 8, 2014, the average citations of each article is 0.75, which means the *impact factor* of these 365 articles is 0.75. Additionaly, the mean citations of the articles published in 2013 is 1.1, and 0.11 for the articles published in 2014 -- of course, calculating the *impact factor* for these recently published articles in 2014 is meaningless. Althought this is a crude calculation, I am sure, several years later, the official impact factor will be similar as PLoS ONE when it was announced, which will be more than 3 points. It is the fact that as the time goes by, the number of citations of each article will increase. 
-	**Distribution of subjects**. PeerJ [only accepts](http://en.wikipedia.org/wiki/PeerJ) the manuscripts from biological or medical sciences. A question comes out: are there any variations in the subjects, or any inclinations for some specific subjects? I listed the first 20 subjects based on the information extraced from these 365 articles, which was shown in the following figure ([download (2KB)](http://sixf.org/files/code/2014/05/subjects.txt) this full list). The first subject is ecology, having 80 published articles with a proportion of 21.92% of these 365 articles, then the evolutionary studies (51 articles) and zoology (50 articles).

![](http://sixf.org/files/images/2014/05/peerj_subjects.png)

-	**[PeerJ PrePrints](https://peerj.com/about/publications/#PeerJ-PrePrints)**. Preprint archive, which is very common in mathmatical or physical sciences, such as the newly well-known research based on a model of "[ston-scissors-cloth](http://news.sciencenet.cn/htmlnews/2014/5/293837.shtm)", which was originally published on [arXiv](http://arXiv.org), another popular preprint website hosted by Cornell University. PeerJ PrePrints is also a preprint website, and you can submit unlimited manuscript to PeerJ Preprint which will be online in couple hours! I have to admit that this is a great improvement, too!
-	**"Full service"**. From my submission to final acceptance, the editorial office of PeerJ alway kept in touch with me. I am glad to say that this submission experience is very pleasant. After the manucsript was accepted, [Jackie Thai](https://peerj.com/about/), the production editor of PeerJ, corrected some grammatical errors in our manuscript -- big thanks to her! Of course, the official website of PeerJ have introduced a lot *why publish your paper on PeerJ*, such as [here](http://blog.peerj.com/post/46261563342/6-reasons-to-publish-with-peerj), or [here](http://blog.peerj.com/post/54500700950/7-reasons-why-peerj-is-the-perfect-conference-publisher
).
-	**Fly in the ointment**. Finally, although the submission system of PeerJ is pretty friendly, I still puzzed when submitting my mansucript. Luckily, I could contact the editorial office for help. Another trouble is the slow speed of openning the PeerJ website or submission, at least, in China. It may cost more than 5 minutes to upload hundreds kilobyte files, even though the submission will frequently failed. Surprisingly, once I failed to upload my manuscript, I was immediately got an email from Jason Hoyt, the CEO of PeerJ, asking if I need any help. At that time, I did want to know is Jason always monitoring the submission system?

**Conclusion**: PeerJ looks somewhat similar as PLoS ONE at the moment, and [some staffs at PeerJ](https://peerj.com/about) also formally worked at PLoS ONE. But, I predict PeerJ will open a new road with its innovative bussiness strategies, and catch up with or even surpass PLoS ONE in the next few years. As a result, for the question of this post, *PeerJ, the next PLoS ONE*, the simple answer is: pupil excels teacher.