![adventure_title](/assets/img/adventure_title.jpg)

This page shows one example of the kinds of research we hope to make available to more scholars by adding to and improving on The Historical TV Guide.

Having published the dataset and this notebook on GitHub, television scholars are able to reproduce our research, and launch studies of their own with the data. To access the dataset and run our Jupyter Notebooks visit the project's dataset on [KiltHub](#insert link) and our [GitHub Repo](https://github.com/dSHARP-CMU/megaText).

## Episode 01 - Working-Class Content in the Action & Adventure Genre

In March 2018, at the Society for Cinema and Media Conference, in Toronto Canada, Newman and Gotzler gave a paper titled “Using the Television 'Mega-text' to Find Social Class in 1950s Television.” To write this paper Newman and Gotzler performed a series of operations on the database they had built pursuing their initial questions about the social class content of 1950s television.

Rather than attempt to analyze the entire dataset for working-class content all at once, we decided to begin our analysis by parsing the data by genre. Genre was attractive to us as a starting point because it ensured we captured a range of programming from different networks, and throughout the decade. 

Figure 1 shows the distribution of genre categories over all of 1950s television, with the most number of television programs belonging to the Variety genre, and the least to the Science Fiction genre. Figure 2 shows six distinct graphs of the frequency of six separate genres over the course of the decade. Notice that Variety genre drops off sharply by the end of the decade, while Crime Dramas end the decade on an upswing.

### Figure 1
![figure1](/assets/img/Figure1.png)

### Figure 2
![figure2](/assets/img/Figure2.png)

For the first round of analysis, Newman and Gotzler chose to examine the Adventure genre for evidence of working class content. 
Adventure was chosen for a number of reasons. First, it was chosen over the more prevalent genres of "Anthology," "Game Show," and "Variety" as the program descriptions of these shows are vague and general--as a result of their changing format--thus, from print sources alone it would be very difficult to glean whether or not these programs contained working-class content. Second, there is relatively less consensus among TV scholars about the class politics of the "Action & Adventure" genre in comparison to other genres such as "Comedy" which scholars have long-studied, especially in relation to the birth of the sit-com and the varying depictions of social class in well-known programs like *I Love Lucy*, *The Honeymooners*, and *Leave it to Beaver*. Finally, "Action & Adventure" was selected because it was, after comedy, the most prevalent conventional narrativer genre in the dataset.

## Creating the Subset 
Using a data-analysis package called “pandas” for the programming language Python3, Newman and Gotzler created a subset of the data for analysis of only those programs that had the "Action" or “Adventure” designation in the data set they had created. This was accomplished by creating a new data frame that captured everything containing either an "Adventure" or "Action" tag in any of the various print sources that had been gathered into the dataset. This brought together a range of programs, many of which he had also been categorized as “Science Fiction” or “Crime Drama,” but that contained either an “Action” or “Adventure” genre tag in their entry metadata from on of the data sources. Figure 3 shows a snapshot of this new data frame for the Action & Adventure subset. Newman and Gotzler then exported this Adventure subset as a spreadsheet to a .csv file and hand-coded each program for working-class content after considering the relevant information such as program description, plot synopsis and summary, etc. 

### Figure 3
![figure 3](/assets/img/Figure3.png)

## Coding for Working-Class Content

To code the Action & Adventure programs Newman and Gotzler developed a taxonomy for descriptive assessments of occupations and settings depicted in the programs. After assigning these descriptive categories, Newman and Gotzler then evaluated each show on a binary scale for whether it contained working-class content or not. Figures 4, 5, and 6 display the taxonomies for each of these codings respectively.

### Figure 4 
![figure 4](/assets/img/Figure4.png)

### Figure 5
![figure 5](/assets/img/Figure5.png)

### Figure 6
![figure 6](/assets/img/Figure6.png)

## Preliminary Results

To analyze the sub-set of coded Adventure programs Gotzler utilized data management and visualization packages (pandas, and matplotlib) in the programming language python3. Gotzler wrote these python scripts into a “Jupyter Notebook” which is a computational environment software that allows you to publish and share your research in ways that enable transparency and reproducibility.

A notebook recording the preliminary analysis of working-class content in programs from the "Action & Adventure" genre over the course of the 1950s, can be found on the project's [GitHub Repo](https://github.com/dSHARP-CMU/megaText), commentary and explanation of the analytical methods and process is provided throughout.
 
**Key Takeaways**

(1) Unsurprisingly, the Adventure genre contains a high number of non-US, non-contemporary settings; these fall into “Historical Period” and “Particular Country (not US)”, but also include “Sci-Fi Fantasy” settings. 

(2) The urban settings in NYC, or other “Particular Cities” -- come mostly from Crime or Detective shows, with “Action” genre tags..

(3) Surprisingly, only one program in the subset we analyzed corresponded to a Western setting. --We are still in the process of double checking, to see if we’re missing something with the capture, as it seems unlikely that more Western shows in IMDB are not genre tagged as “Adventure” or “Action”
  
After generating these initial coded counts, programs were grouped by **Occupation+Working-Class Content=YES**, and **Setting+Working-Class Content YES**. 

Figures 7 and 8 represent the results of Newman and Gotzler’s coding of the Adventure genre according to its working class content. The color orange correlates with programs that we deemed as having primarily working class content and the color blue correlates with programs that we deemed as having primarily middle class content. 

For example, in Figure 7, we catalogued nineteen unique occupation types in the programs within the Adventure genre. Some of the programs that contained these occupations we categorized as working class, while others we categorized as middle class, while still others had elements of both. For example, where we found foresters, spies, scientists and newspaper reporters, we classified all of those programs as having middle class or other in content. But where we found construction workers, criminals, transportation workers and police, we classified all of those programs as having working class content. Where we found “crime solving (informal)” we found programs that we coded as both working class, as well as middle class or other.

### Figure 7
![figure 7](/assets/img/Figure7.png)

Figure 8 shows what happened when we grouped by setting instead of occupation. For example, programs featuring the Western setting or programs that were oriented to children we classified as primarily middle class. Programs with an outdoor setting were predominantly working class. The setting of New York city produced both middle class and working class Adventure programs.

### Figure 8
![figure 8](/assets/img/Figure8.png)

Some interesting patterns also emerged from this analysis:

(1) The highest coincidence (in terms of overall share of programming) of working-class content and a single occupation occurred in programs featuring “Crime Solving (informal)” 

(2) The highest coincidence of working-class content and a single setting occurred in programs set in a “Historical Period” -- nearly half of each.

**Crime Solving (informal)**

A high proportion of adventure programs contained characters whose job involved battling injustice without any other mention of more formal employment, and where the character was not a policeman, a superhero, a detective or a private investigator. These crime solvers were precarious in their relationship to capital as well. In many of these programs it is not clear who hired them, or from whence their livelihoods came. In coding the adventure subset we developed the category of "Crime Solving (informal)" to capture these occupations.

A prime example of this somewhat ambiguous occupational category can be found in a short-lived program from 1952 *The Affairs of China Smith*, which you can see the details of here:

> #### *The Affairs of China Smith* (1952)
>
> #### <u>Program Description:</u> China Smith is a daring American soldier of fortune living in Singapore. China takes what cases he needs to survive and while he dislikes doing it, he always finds himself handing out freebies--helping innocent people who become involved with unscrupulous characters (sometimes as the result of a case he is investigating for the government). Cast: Dan Duryea (China Smith).
>
> #### <u>Program Genre:</u> Adventure, Action, Drama
> #### <u>Setting_Type:</u> “Particular Country (not US)”
> #### <u>Occupation_Type:</u> “Crime-Solving (informal)”
> #### <u>Evaluation_ID:</u> “Working_Class_YES”

**Historical Period**

It is also curious that so many of the programs which appear to contain working-class content would be set in historical periods. These occasionally reached as far back as the medieval period pre-capitalist eras romances, but also included programs set during the Old West, or other parts of the nineteenth century. This is somewhat surprising given the assumption that conventional historical sense elides the presence of class conflict or working-class culture. However it is also quite fitting, as in some sense it reveals the inability to imagine a narrative of history that isn't rooted in class struggle. 

A good example of a single record in the dataset that exhibits both of these trends is, “The Adventures of Robin Hood”, which you can see the details of here:

>#### *The Adventures of Robin Hood* (1955-1958)
>
>#### <u>Program Description:</u> "Robin Hood, Robin Hood, riding through the glen; Robin Hood, Robin Hood, with his band of Merry Men; feared by the bad, loved by the good, Robin Hood...." The series, set in 11th century England, relates the adventures of Robin Hood, the most celebrated of outlaws (who stole from the rich to give to the poor) and his band of Merry Men (free-born Englishmen loyal to the king who have established a base of operations in Sherwood Forest)...
>
>#### <u>Program Genre:</u> “Adventure”, “Action”, “Family”
>#### <u>Setting_Type:</u> “Historical Period”
>#### <u>Occupation_Type:</u> “Crime Solving (informal)
>#### <u>Evaluation_id:</u> Working_Class_YES



### [Return](/Historical-TV-Guide)
