# Web Scrape Popular Topics and Repository in GitHub
## Libraries Used
- `requests` library to download the “Topics on GitHub” page,
- `BeautifulSoup` library to parse and extract information like top topics and repositories under each topic with details
- `Pandas` to convert into a final dataframe.
### Steps
1. Scrape https://github.com/topics
2. Get a list of all topics. For each topic, get topic `title`, topic page `URL` and topic `description`
3. For each topic, Get the top 25 repositories in the topic from the topic page
4. For each repository, Grab the repo `name`, `username`, `stars` and repo `URL`
5. At last create a CSV file by compling all scraped data
---
## Scraping Popular GitHub Topics
### Topics Dataframe Attributes:
1. `title` - Name of the topic - [3D]
2. `description` - Description of that topics - [3D modeling uses specialized software to create a digital model of a physical object. It is an aspect of 3D computer graphics, used for video games, 3D printing, and VR, among other applications.]
3. `url` - URL of that topic - [https://github.com/topics/3d]
---
## Scraping Top 30 Repositories Under Each Topic
### Repo Dataframe Attributes:
1. `repo_name` - Name of the repository
2. `username` - Owner of that repository
3. `stars` - Stars on that repository
4. `repo_url` - URL of that repository
---
