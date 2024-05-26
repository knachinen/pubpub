---
title: scraping - 001 - timeover
tags:
  - web-scraping
  - time-over
  - darkmap
  - python
---

selenium 으로 웹 스크래핑을 하는데,  
페이지 로딩이 오래 걸리거나,  문제가 있는 경우,  
다음 iteration 으로 넘어가지 못한다.  

이럴때, 간단하게 시간제한으로 넘기도록 하였다.  


```python
def timeout_handler(num, stack):
    raise Exception("TIMEOVER")

def set_alarm(duration: int):
    signal.signal(signal.SIGALRM, timeout_handler)
    signal.alarm(duration)

for index in tqdm(self.index_url):
	url = self.df.loc[index, "URL"]
	try:
		set_alarm(10)
		result = self.get_html_selenium(url=url, driver=driver)
	except Exception as ex:
		result = 'timeout'
	finally:
		signal.alarm(0)
	self.df.at[int(index), new_column_name] = str(result)

```