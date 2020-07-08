# **The correlation between user rating score and content for the audience by age group.**
Concerning this dataset and due to the vast amount of time it would take to collect 1,000 shows one by one; the individual gathered method preyed on Netflix’s suggestion engine. The suggestion engine recommends shows like those selected in this dataset.  *"As part of this data set, I took 4 videos from 4 ratings (totaling 16 unique shows), then pulled 53 suggested shows per video. The ratings include G, PG, TV-14, TV-MA. I chose not to pull from every rating (e.g. TV-G, TV-Y, etc.). "*- Chase Willden

# **Part 1 - Load and Validate the Data**

*  Load the data as a pandas data frame.
*  Validate that it has the appropriate number of observations (checking the raw file, and also read the dataset description from data.world [Netflix](https://data.world/chasewillden/netflix-shows/workspace/file?filename=netflix.xlsx) ).

source: data.world [Netflix Suggestion Engine](https://data.world/chasewillden/netflix-shows)


**Setup:**

```
Jupyter notebook
text editor
or
Google Colab
```


**Import Statements:**
```
# Let's begin by importing pandas
# We also imported numpy, matplotlib, and seaborn

#classics
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

```


```
# We use the pandas method pandas.read_csv("filepath") to create a DataFrame 
# and assign it to a variable df.
# We'll use the head() method, which by default prints out the first 5 rows. 
# We're supposed to have 1000 observations (rows) and seven columns. 

pd.options.display.max_rows=999
pd.options.display.max_columns=100

df=pd.read_csv("netflix-netflix-shows-QueryResult.csv")

df.replace("?", np.NaN)
print(df.shape)
df.head()
```

# **Part II - Data Exploration**
> *First, I wanted to see if Netflix had a diverse library of content with the array of ratings. I found within the dataset that they have twelve categorical ratings, ranging from G to TV-MA.*
![alt text](https://miro.medium.com/max/1220/1*Y5gRPAP82yyE_xq__eUXQA.png)

The rating system from [Netflix](https://help.netflix.com/en/node/2064) indicates how the audience it's broken down by rating:
        
*   Little Kids G, TV-Y, TV-G
*   Older Kids PG, TV-Y7, TV-Y7-FV, TV-PG
*   Teens PG-13, TV-14
*   Mature R, NC-17, TV-MA

        
another source: [Film Ratings](https://www.filmratings.com/)
# **Part III - Visulizations**


### want to get in touch?

*  [Linkedin](https://www.linkedin.com/in/jorgelima/)
*  [Twitter](https://www.twitter.com/thisisjorgelima/)
*  [Podcast](https://mailchi.mp/db9640dec7a5/a-month-of-saturdays)
*  [Instagram](https://www.instagram.com/thisisjorgelima/)
*  [Facebook](https://www.facebook.com/thisisjorgelima/)
*  [Website](https://www.thisisjorgelima.com/)
*  [Github](https://www.github.com/thisisjorgelima/)
                                                                           
### You can applaud my story on Medium here:
[Medium](https://medium.com/@ThisIsJorgeLima/the-correlation-between-user-rating-score-and-content-for-the-audience-by-age-group-4539a9f230a7)

### Here is a link to my code:
[Code](https://colab.research.google.com/drive/1jzKf7goCdi4RGpqWJfwaNYY8JI2gV2sH)

## License

[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2019-2020 © <a href="http://thisisjorgelima.com" target="_blank">Jorge A. Lima</a>.
 
