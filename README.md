# Collecting-Data-Assignment-3
Henry Hornung (S4156145)

## Data
For this assignment, I decided to scrape a corpus from the internet consisting of poems written by the author HP Lovecraft. The poems were scraped from https://www.hplovecraft.com/, an online archive and biography revolving around HP Lovecraft and his works. While Lovecraft wrote hundreds of poems in his lifetime, 49 of them have been digitized and made available on the website.

## Processing
Initially, I scraped the titles of each poem from this site, https://www.hplovecraft.com/writings/texts/, and saved them in a list. Since they contained hyperlinks to each poem's respective site, I was able to scrape those too and put them into another list. Then, using the hyperlinks, I wrote a code that applied the same scraping and cleaning parameters to each link through the use of a for-loop. These consisted of removing any spacing elements or tags, and joining the text into one body if it was split. Through the cleaning of the text, all line breaks and indents were removed, making it easier to read for machines. I then saved each poem in a third list. At the same time, I created a fourth list which contained the poems with their original structuring in tact, allowing humans to read them more easily, and as intended by the author. Finally, I created a dataframe with the titles, poems and links. This dataframe was exported as "HP_Lovecraft_Poems.csv" and can be found in the git repository.

## CSV Key
||Title|Text_Original|Text_Continuous|Link|
|---|---|---|---|---|
|Contains the poem/row count.|Contains the title of the poem.|Contains the poem itself, in its original form.|Contains the poem itself, with all indents and line breaks removed.|Contains the hyperlink to the page that the poem was scraped from.|


## Permissions
The website itself had no terms or conditions, nor did it have a "robot" file. The website is a non-official project run by three individuals who have no affilliation to Lovecraft's estate. Furthermore, since Lovecraft died more than 70 years ago, his work how falls under the public domain, and can as such be used for this project.
