# Culinary trip around the world without leaving Berlin

## 1. Description
Being very interested in different cuisines and cultures but without the resources to travel around the whole world, my question was whether it was possible to visit all countires in the world through their cuisine while being in Berlin. For that I collected data from the Foursquare's API.

## 2. Results
- Almost 50% of the countries have a restuarant in Berlin that represents their cuisine.![](visualizations/Map_countries_no_restaurants.png)
- The continent with more restaurants representing their cuisine is Asia. ![](visualizations/Restaurants_per_continent.png)
- However, the cuisine with the most restaurants is Italian cuisine. This can be due to the amount of asian fusion restaurants which divides the number of restaurants and therefore they end up having fewer restaurants than Italy.![](visualizations/Top_10_countries.png)
- With Ironhack as the starting point, I've created and optimized a route to visit one restaurant of each country, one after the other as we would be travelling around the globe. With Here's API I have obtained the directions to get from one place to the next, the time needed and the public transportation routes. ![](visualizations/route_optimized_every_country.png)
- Since usually one only wants to eat in one restaurant per day. I have represented the closest restaurant to Ironhack for each type of cuisine.![](visualizations/closest_restaurant_every_country.png)
- I have also created and optimized a route for each continent. Meaning, visiting all restaurants available with cuisine belonging to a specific continent. Below South America is used as example ![](visualizations/route_optimized_continent.png)
- Lastly, I have created a small tool with which one can give ones location (latitude and longitude) and the type of cuisine that one is interested in, and all restaurants belonging to that cuisine will be displayed in a map, together with a line joining that restaurant with the given location. Below Brazilian cuisine is used as example ![](visualizations/closest_restaurants_to_location.png)

## 3. Files
- data_prep: gets the data from Foursquare's API, cleans it and processes it so that it can be later used for the visualization and analysis parts, then exports several pickle files.
- Analysis: notebook used to visualize and get the above-mentioned results. The following visualizations are produced:
  - Geographic distribution of the restaurants
  - Top 10 country-cuisines with the most restaurants in Berlin
  - Distribution of restaurants per continent
  - Percentage of countries represented vs countries not represented
  - Map visualization of countries represented and the number of restaurants
- Routing: notebook containing all the optimization routes, getting directions from Here's API, visualizing the results on a map and exporting several pickle and csv files.
- data: folder where all pickle and csv files are being exported to
- input: folder that contains two csv files needed in the data-prep notebook
- visualizations: folder containing screenshots of the graphs made with plotly express (they aren't rendered in github)

## 4. Sources
- [Foursquare's API](https://de.foursquare.com) for getting a dataset of restaurants 
- [Here's API](https://www.here.com) for getting directions

## 5. Environment dependencies
- appnope==0.1.0
- asn1crypto==1.2.0
- attrs==19.3.0
- backcall==0.1.0
- beautifulsoup4==4.8.1
- bleach==3.1.0
- certifi==2019.11.28
- cffi==1.13.2
- chardet==3.0.4
- coverage==4.5.4
- cryptography==2.8
- cycler==0.10.0
- decorator==4.4.1
- defusedxml==0.6.0
- entrypoints==0.3
- holidays==0.9.11
- idna==2.8
- importlib-metadata==0.23
- ipykernel==5.1.3
- ipython==7.9.0
- ipython-genutils==0.2.0
- ipywidgets==7.5.1
- jedi==0.15.1
- Jinja2==2.10.3
- joblib==0.14.0
- jsonschema==3.2.0
- jupyter==1.0.0
- jupyter-client==5.3.4
- jupyter-console==6.0.0
- jupyter-core==4.6.1
- kiwisolver==1.1.0
- MarkupSafe==1.1.1
- matplotlib==2.2.4
- mistune==0.8.4
- mkl-fft==1.0.15
- mkl-random==1.1.0
- mkl-service==2.3.0
- more-itertools==7.2.0
- nbconvert==5.6.1
- nbformat==4.4.0
- notebook==6.0.2
- numpy==1.17.4
- ortools==7.4.7247
- packaging==19.2
- pandas==0.25.3
- pandocfilters==1.4.2
- parso==0.5.1
- patsy==0.5.1
- pexpect==4.7.0
- pickleshare==0.7.5
- plotly==4.3.0
- plotly-express==0.4.1
- pluggy==0.13.1
- pprintpp==0.4.0
- prometheus-client==0.7.1
- prompt-toolkit==2.0.10
- protobuf==3.11.1
- ptyprocess==0.6.0
- py==1.8.0
- pycountry==19.8.18
- pycountry-convert==0.7.2
- pycparser==2.19
- Pygments==2.4.2
- PyMySQL==0.9.3
- pyOpenSSL==19.1.0
- pyparsing==2.4.5
- pyrsistent==0.15.6
- PySocks==1.7.1
- pytest==5.3.1
- pytest-cov==2.8.1
- pytest-mock==1.12.1
- python-dateutil==2.8.1
- pytz==2019.3
- pyzmq==18.1.0
- qtconsole==4.6.0
- repoze.lru==0.7
- requests==2.22.0
- retrying==1.3.3
- scikit-learn==0.21.3
- scipy==1.3.1
- seaborn==0.9.0
- Send2Trash==1.5.0
- six==1.13.0
- soupsieve==1.9.5
- statsmodels==0.10.1
- terminado==0.8.3
- testpath==0.4.4
- tornado==6.0.3
- traitlets==4.3.3
- urllib3==1.24.2
- wcwidth==0.1.7
- webencodings==0.5.1
- widgetsnbextension==3.5.1
- zipp==0.6.0
