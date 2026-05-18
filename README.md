# DSA 210 Project: The Effect of Animated Thumbnails on Video Game Mods Metrics

> [!NOTE]
> Please consider checking *DSA 210 Project Final Report.pdf* for a more detailed overview.

## Motivation
I am a video game mod developer actively working on creating mods for a game called Garry’s Mod. For the past several years I have noticed a growing trend in the way mod (addon) representations are made in the Steam Workshop, the main modding platform provided within Steam by Valve. Increasingly addons are starting to move towards animated thumbnails, presumably for more attention or just following a trend.

This project is dedicated to potentially revealing the underlying reason behind the surge of animated thumbnails compared to the dominant static thumbnail formats of the past.

## Data Source
All data comes from the Steam Workshop's built in telemetry. These include visitors, subscribers, favorites, collections, comments, ratings and much more. Some information is only accessible to mod authors which significantly limits the reach of external research (private numbers). The table below shows the data features based on accessibility level.

| Public Numbers | Private Numbers |
| ---------------- | --------------- |
| Current Subscribers | Total Unique Subscribers |
| Current Favorites | Total Unique Favorites |
| Total Ratings | Positive Ratings |
| Unique Visitors | Negative Ratings |
| # of Comments | Cumulative Subscribers |
| # of Collections | Views and ratings over time |

Two datasets were created. The first one is made out of 100 public mods and the second is made from 34 of my own mods. The public dataset was enriched by including all 10 addon types present in the Workshop. Check the Datasets folder in the repo or the final report document for links to the datasets.

## Data Analysis
Heavy use of hypothesis testing was made to evaluate all available features on both datasets. Linear regression was also conducted on the private dataset for the cumulative subscribers feature.

## Findings
The public dataset did not reveal any significant information but the private dataset showed some features were significantly affected:

| Significant Numbers | Insignificant Numbers |
| ---------------- | --------------- |
| Unique Visitors | Current Favorites |
| Current Subscribers | Comments |
| Collections | Negative Ratings |
| Stars | Unique Subscribers |
| Positive Ratings | Unique Favorites |

Linear regression also revealed that animated thumbnails received more average subscribers in the first 60 days compared to static thumbnails though subscriber retention and increase are very similar.

## Limitations and Future Work
Web scraping was desired but could be conducted due to time constraints severely affecting dataset size and quality. The "Views and ratings over time" data could not be used and linear regression could have been replaced with multinomial regression instead. Also the findings from the private dataset might not represent the entire Workshop accurately. Despite all this I consider this project a good start into the analysis of a very unexplored field.

## AI Disclosure
No generative AI and/or LLM tools were used in any part of the project.
