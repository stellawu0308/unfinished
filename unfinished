import hello
from hello import get_soup
get_soup('https://tw-nba.udn.com/nba/cate/6754')
url='https://tw-nba.udn.com/nba/cate/6754'
soup=get_soup(url)
def Get_news():
    cfs=soup.find(id="news_list_body").find_all('div', class_="box_body")
    for cf in cfs:
        title=cf.find('h3').text.strip()
        source=cf.find('b').text
        content=cf.find('p').text
        image=cf.find('img').get('src')
        print(title,source,content,image)
Get_news()
