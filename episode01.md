 
This page shows one example of the kinds of research we hope to make available to more scholars by adding to and improving on The Historical TV Guide.

Having published the dataset and this notebook on GitHub, television scholars are able to reproduce our research, and launch studies of their own with the data. To access the dataset and run our Jupyter Notebooks visit the project's dataset on [KiltHub]{#insert link) and our [GitHub Repo](#insert link).

## Episode 01 - Working-Class Content in the Action & Adventure Genre

In March 2018, at the Society for Cinema and Media Conference, in Toronto Canada, Newman and Gotzler gave a paper titled “Using the Television 'Mega-text' to Find Social Class in 1950s Television.” To write this paper Newman and Gotzler performed a series of operations on the database they had built pursuing their initial questions about the social class content of 1950s television.

Rather than attempt to analyze the entire dataset for working-class content all at once, we decided to begin our analysis by parsing the data by genre. Genre was attractive to us as a starting point because it ensured we captured a range of programming from different networks, and throughout the decade. 

*Figure 1* shows the distribution of genre categories over all of 1950s television, with the most number of television programs belonging to the Variety genre, and the least to the Science Fiction genre. *Figure 2* shows six distinct graphs of the frequency of six separate genres over the course of the decade. Notice that Variety genre drops off sharply by the end of the decade, while Crime Dramas end the decade on an upswing.

### Figure 1
[Insert inline image ADD genre graphics]

### Figure 2
[insert inline image]

For the first round of analysis, Newman and Gotzler chose to examine the Adventure genre for evidence of working class content. Newman and Gotzler chose the Adventure genre to start with, hypothesizing that they would find more working class characters, occupations, and settings in the Adventure dramas than in other genres such as Game Shows or Comedy.
*add further justification about Genre (comedy vs. adventure, and break-down of prevalence)

## Creating the Subset 
Using a data-analysis package called “pandas” for the programming language Python3, Newman and Gotzler created a subset of the data for analysis of only those programs that had the "Action" or “Adventure” designation in the data set they had created. This created a new data frame to work with, and allowed them to capture everything Terrace had coded as “Adventure” but also brought in other programs, many of which he had categorized as “Science Fiction” or “Crime Drama,” but that contained either an “Action” or “Adventure” genre tag in their entry metadata on IMDB. Newman and Gotzler then exported this Adventure subset as a spreadsheet to a .csv file and hand-coded each program for working-class content after considering the relevant information such as program description, plot synopsis and summary, etc. 

To code the television programs Newman and Gotzler developed a taxonomy for descriptive assessments of occupations and settings depicted in the programs. After assigning these descriptive categories, Newman and Gotzler then evaluated each show on a binary scale for whether it contained working-class content or not. 

[insert image of working-class content table]

[insert image of settings and occupations tables] 

#### Working-Class Content
[ADD inline image] Working Class Content: NO or YES (1 or 2, binary code scale)

#### Occupation 
[ADD INLINE IMAGE] Occupation: Transportation, Forestry, Construction, Scientist, or Detective

#### Setting
[ADD inline image] Setting: Sci-Fi Fantasy, West (Western), or Historical Period, 


##Re-number figures in document subsequent to these inserted tables.

To analyze the sub-set of coded Adventure programs Gotzler utilized data management and visualization packages (pandas, and matplotlib) in the programming language python3. Gotzler wrote these python scripts into a “Jupyter Notebook” which is a computational environment software that allows you to publish and share your research in ways that enable transparency and reproducibility. Our notebook records our preliminary analysis of working-class content in programs from the action adventure genre over the course of the 1950s. Commentary and explanation on our analytical methods and process is provided throughout.
 
In the course of this analysis Newman and Gotzler discovered a new occupation that was very common in the Adventure genre, an occupation they have labeled “Crime Solving (informal)”.. A high proportion of adventure programs contained characters whose job involved battling injustice without any other mention of more formal employment, and where the character was not a policeman, a superhero, a detective or a private investigator. These crime solvers were precarious in their relationship to capital—in many of these programs it is not clear who hired these informal crime solvers, or from whence their livelihoods came.

*Figures 4 and 5* represent the results of Newman and Gotzler’s coding of the Adventure genre according to its working class content. The color orange correlates with programs that we deemed as having primarily working class content and the color blue correlates with programs that we deemed as having primarily middle class content. For example, in *Figure 4*, we catalogued nineteen unique occupations types in the programs within the Adventure genre. Some of the programs that contained this occupation we categorized as working class, while others we categorized as middle class, while still others had elements of both. For example, where we found foresters, spies, scientists and newspaper reporters, we classified all of those programs as having middle class content. But where we found construction workers, criminals, transportation workers and police, we classified all of those programs as having working class content. Where we found “crime solving (informal)” we found programs that we coded as being primarily working class, as well as programs we coded as primarily middle class.

*Figure 5* shows what happened when we isolated setting instead of occupation. For example, programs featuring the Western setting or programs that were oriented to children we classified as primarily middle class. Programs with an outdoor setting were predominantly working class. The setting of New York city produced both middle class and working class Adventure programs. 

### Preliminary Results

In our preliminary results, when programs were grouped by [Occupation+Working-Class Content YES], and [Setting+Working-Class Content YES], some interesting patterns emerged.

(1) The highest coincidence (in terms of overall share of programming) of working-class content and a single occupation occurred in programs featuring “Crime Solving (informal)” -- and the highest coincidence of working-class content and a single setting occurred in programs set in a “Historical Period” -- nearly half of each.

(2) A good example of a single record that exhibits all these trends is, “The Adventures of Robin Hood”, which you can see the details of here.

**Key Takeaways**
(1) Unsurprisingly, the Adventure genre contains a high number of non-US, non-contemporary settings; these fall into “Historical Period” and “Particular Country (not US)”, but also include “Sci-Fi Fantasy” settings. 

(2) The urban settings in NYC, or other “Particular Cities” -- come mostly from Crime or Detective shows, with “Action” genre tags..

(3) Surprisingly, only one program in the subset we analyzed corresponded to a Western setting. --We are still in the process of double checking, to see if we’re missing something with the capture, as it seems unlikely that more Western shows in IMDB are not genre tagged as “Adventure” or “Action”


>**Closer Look - “Historical Period”**
>
>*The Adventures of Robin Hood (1955-1958)*
>
>**Program Description**:  "Robin Hood, Robin Hood, riding through the glen; Robin Hood, Robin Hood, with his band of Merry Men; feared by the bad, loved by the good, Robin Hood...." The series, set in 11th century England, relates the adventures of Robin Hood, the most celebrated of outlaws (who stole from the rich to give to the poor) and his band of Merry Men (free-born Englishmen loyal to the king who have established a base of operations in Sherwood Forest)...
>
>**Program Genre**: “Adventure”, “Action”, “Family”
>
>**Setting_Type**: “Historical Period”
>**Occupation_Type**: “Crime Solving (informal)
>**Evaluation_id**: Working_Class_YES

INSERT FURTHER INFO FROM SLIDES and NEH GRANT IMAGES

### [Return](/Historical-TV-Guide)
