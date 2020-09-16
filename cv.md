# Vitali Serada
![Image of Vitali Serada](https://sun9-68.userapi.com/impg/c857424/v857424987/12a7a5/7u2VAnY_FUo.jpg?size=400x0&quality=90&sign=c325b88989e831245e712ee3e444a950)
### Contact info
* mobile: +375291724505 
* e-mail: serada.vitali@yandex.ru 
* telegram: vitalikreykjavik 

### Summary
My goal is to become a worthy specialist in every field where I try my hand. Unfortunately, in my current profession I have reached a maximum on the career ladder and do not see further development. Therefore, I decided to study one of the areas of IT, because, first of all, it is a highly competitive sphere with almost unlimited possibilities for progression. I am also attracted by the need for constant study in order to keep up with the industry. And the last: this sphere is developing rapidly and, in my opinion, will be decisive in the future.
I am a quick and easy leaner, stress-resistant and self motivated, get alone with any team, team player. 

### Skills
HTML/CSS basics, Python basics, Pandas basics, GIT, Jupyter Notebook, macOS, Windows

### Code example
```python
import pandas as pd
df = pd.read_csv('/datasets/music_project.csv')

df.head(10)
df.dtypes
df.columns
df.set_axis(['user_id','track_name','artist_name','genre_name','city','time','day'], axis='columns', inplace=True)
df.isnull().sum()
df['track_name'] = df['track_name'].fillna('unknown')
df['artist_name'] = df['artist_name'].fillna('unknown')
df.isnull().sum()
df.dropna(subset = ['genre_name'], inplace=True)
df.isnull().sum()
df.duplicated().sum()
df.drop_duplicates().reset_index(drop=True)
df.duplicated().sum()
genres_list = df['genre_name'].unique()
def find_genre(genre):
    count = 0
    for i in genres_list:
        if genre == i:
            count += 1
    return count
find_genre('hip')
find_genre('hop')
find_genre('hip-hop')
def find_hip_hop(dataframe, wrong_genre_name):
    dataframe['genre_name'] = dataframe['genre_name'].replace(wrong_genre_name, 'hiphop')
    result = dataframe[dataframe['genre_name'] == wrong_genre_name].count()
    result1 = result.count()
    return result
find_hip_hop(df, 'hip')

df.info()

df.groupby('city')['genre_name'].count()
df.groupby('day')['genre_name'].count()

def number_tracks(dataframe, weekday, what_city):
    track_list = dataframe[(dataframe['day'] == weekday) & (dataframe['city'] == what_city) ]
    track_list_count = track_list['genre_name'].count()
    return track_list_count
    
number_tracks(df, 'Monday', 'Moscow')

data = [['Moscow', 16299, 11547, 16610],
       ['Saint-Petersburg', 5882, 7379, 6164]]
columns = ['city', 'monday', 'wednesday', 'friday']
assss = pd.DataFrame(data = data, columns = columns)
```

### Experience
* HTML/CSS courses ([HTML академия](http://htmlacademy.ru), [Code School](http://codeschool.com))
* Data analyst courses ([Яндекс Практикум](http://praktikum.yandex.ru))

### Education
* 2008-2013: BSU, Oriental (Chinese) languages. Specialist, philological. GPA: 8,9 out of 10.
* 2010: Dalian University of Technology (China): Monthly courses of Chinese language and culture.
* 2011-2012: Dalian University of Technology (China): Annual courses of Chinese language and culture.
* HTML/CSS courses
* Data analyst courses  

### Languages 
* English B1-B3 - permanent use at work, mainly written speech
* Chinese C1 - main working tool, permanent use at work