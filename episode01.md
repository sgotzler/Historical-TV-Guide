Rather than attempt to analyze the entire dataset for working-class content all at once, we decided to begin our analysis by parsing the data by genre. Genre was attractive to us as a starting point because it ensured we captured a range of programming from different networks, and throughout the decade. 

We conducted our analysis using the data management and visualization packages (pandas, and matplotlib) for Python3. We wrote and ran these python scripts in a Jupyter Notebook. Jupyter Notebooks is a computational environment software, that allows you to publish and share your research in ways that enable transparency and reproducibility. Our notebook records our preliminary analysis of working-class content in programs from the action adventure genre over the course of the 1950s. Commentary and explanation on our analytical methods and process is provided throughout.

Having published the dataset and this notebook on GitHub, television scholars are able to reproduce our research, and launch studies of their own with the data. To access the dataset and run our Jupyter Notebooks visit the project's [GitHub Repo](#insert link)

### Episode 01 - Action & Adventure 

**Parsing by Genre**




### Creating a Subset

Working with python3 in Jupyter we were able to use “Boolean Indexing” and “String Handling” to create a new smaller database specifically for adventure. 

This gave us a new data frame to work with, and allowed us to capture everything Terrace had coded as “Adventure” but also brought in other programs, many of which he had categorized as “Science Fiction” or “Crime Drama,” but that contained either an “Action” or “Adventure” genre tag in their entry metadata on IMDB.

### Coding for Working-Class Content

To analyze the television programs in our subset for working class content, we developed a taxonomy for qualitative assessments of both occupations, and settings depicted in the programs. After assigning these descriptive categories, we then evaluated each show on a binary scale for whether it contained working-class content or not.

The taxonomy for this work included:

#### Occupation 
[ADD INLINE IMAGE] Occupation: Transportation, Forestry, Construction, Scientist, or Detective

#### Setting
[ADD inline image] Setting: Sci-Fi Fantasy, West (Western), or Historical Period, 

**Key Takeaways**
(1) Unsurprisingly, the Adventure genre contains a high number of non-US, non-contemporary settings; these fall into “Historical Period” and “Particular Country (not US)”, but also include “Sci-Fi Fantasy” settings. 

(2) The urban settings in NYC, or other “Particular Cities” -- come mostly from Crime or Detective shows, with “Action” genre tags..

(3) Surprisingly, only one program in the subset we analyzed corresponded to a Western setting. --We are still in the process of double checking, to see if we’re missing something with the capture, as it seems unlikely that more Western shows in IMDB are not genre tagged as “Adventure” or “Action”


#### Working-Class Content
[ADD inline image] Working Class Content: NO or YES (1 or 2, binary code scale)
*NOTE: these were hand coded and adjudicated by Prof. Newman and PhD Candidate Gotzler

### Preliminary Results

In our preliminary results, when programs were grouped by [Occupation+Working-Class Content YES], and [Setting+Working-Class Content YES], some interesting patterns emerged.

(1) The highest coincidence (in terms of overall share of programming) of working-class content and a single occupation occurred in programs featuring “Crime Solving (informal)” -- and the highest coincidence of working-class content and a single setting occurred in programs set in a “Historical Period” -- nearly half of each.

(2) A good example of a single record that exhibits all these trends is, “The Adventures of Robin Hood”, which you can see the details of here.

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
