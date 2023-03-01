# 2017-18 ISU World Standings Singles Men
The goal of this project (which is an assignment for my I 310D: Introduction to Human-Centered Data Science class) was to construct and analyze data regarding the official ISU standings of competitive figure skaters during the figure skating season of 2017-18 that I scraped from Wikipedia. The site I scraped from to obtain my table data was the [2017-18 ISU World Standings for Men's Singles Wikipedia Page](https://en.wikipedia.org/wiki/2017–18_ISU_World_Standings#Men's_singles_(213_skaters)), and to read through the data and display the trends I established, I used [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/), [Pandas](https://pandas.pydata.org/docs/), [NumPy](https://numpy.org/doc/), [SciPy](https://docs.scipy.org/doc/scipy/), and [MatPlotLib](https://matplotlib.org/stable/index.html).

The data types and descriptions for the attributes in my data are as follows:

**index**: the original row index for each entry (integer)

**rank**: the rank/standing of the specific figure skater (integer)

**nation**: the nation of origin of the specific figure skater (string)

**skater**: the name of the specific figure skater (string)

**points**: the points awarded to the specific figure skater based on the skater's competitive results (integer)

The ISU states that the algorithm used to obtain skaters' respective points is an "objective merit-based scoring" that is determined based on a skater's competition results of the preceding two seasons and the current season, and remains the basis for the draws at ISU events and part of the criteria for the selection of competitors for the ISU Grand Prix of Figure Skating and other ISU events designated by the ISU Council. Any fault regarding possible bias in point awardment lies with the algorithm.

### Analysis

The histogram that displays the trend of points distribution between skaters is right-skewed, with a long tail on the left side of the graph. There are more than 100 skaters who had a ranking score of 0-500, there are three skaters who had a ranking score of 4000-5000, and there are only two skaters who had a ranking score of at least 5000.

The top three countries that have the most active skaters are Japan ("JPN"), United States ("USA"), and Russia ("RUS"). Russia has the most active skaters, followed by the United States, and then followed by Japan. Many countries only have one active skater, such as Latvia ("LAT"), Uzbekistan ("UZB"), Philippines ("PHI"), Azerbaijan ("AZE"), and Thailand ("THA"), among others.

As the rank number of a figure skater goes up (actual rank goes down), the less points the skater has. The graph that displays this trend resembles an exponential graph with a rate of growth that is less than 1. With lower rank numbers (higher actual ranks), the points are more dispersed and far apart, and with higher rank numbers (lower actual ranks), the points are closer and crowded together.

The mean, median, and quartiles of the box plot that displays the trend of points distribution between skaters are centered around the 1000 mark value. There are no outliers on the lower end, but there are many on the upper end.

### MIT License

Copyright (c) 2023 rosalynlu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

### Creative Commons Attribution-ShareAlike License

Copyright (c) 2023 rosalynlu

Attribution

To re-distribute a text page in any form, provide credit to the authors either by including a) a hyperlink (where possible) or URL to the page or pages you are re-using, b) a hyperlink (where possible) or URL to an alternative, stable online copy which is freely accessible, which conforms with the license, and which provides credit to the authors in a manner equivalent to the credit given on this website, or c) a list of all authors. (Any list of authors may be filtered to exclude very small or irrelevant contributions.) This applies to text developed by the Wikipedia community. Text from external sources may attach additional attribution requirements to the work, which should be indicated on an article's face or on its talk page. For example, a page may have a banner or other notation indicating that some or all of its content was originally published somewhere else. Where such notations are visible in the page itself, they should generally be preserved by re-users.

Copyleft/Share Alike

If you make modifications or additions to the page you re-use, you must license them under the Creative Commons Attribution-Share-Alike License 3.0 or later.

Indicate changes

If you make modifications or additions, you must indicate in a reasonable fashion that the original work has been modified. If you are re-using the page in a wiki, for example, indicating this in the page history is sufficient.

Licensing notice

Each copy or modified version that you distribute must include a licensing notice stating that the work is released under CC-BY-SA and either a) a hyperlink or URL to the text of the license or b) a copy of the license. For this purpose, a suitable URL is: [http://creativecommons.org/licenses/by-sa/3.0/](https://creativecommons.org/licenses/by-sa/3.0/)

For further information, please refer to the [legal code of the CC-BY-SA License](https://creativecommons.org/licenses/by-sa/3.0/legalcode).
