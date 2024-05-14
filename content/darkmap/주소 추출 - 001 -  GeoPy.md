---
title: 주소 추출 - 001 - GeoPy
tags:
  - python
  - darkmap
  - civic-hack
  - geopy
---

데이터 라벨링 작업에서 사건 장소의 주소를 위도, 경도 값으로 입력해야 했다.  
주소를 위도, 경도로 추출하는 작업은, 다음과 같은 코드로 간단하게 할 수 있었다.  

```python
from geopy.geocoders import Nominatim

geolocator = Nominatim(user_agent="my_geocoder")
location = geolocator.geocode(location_name)

if location:
	latitude = location.latitude
	longitude = location.longitude
```

- [GeoPy](https://geopy.readthedocs.io/en/stable/)
- [Geocoders](https://geopy.readthedocs.io/en/stable/#module-geopy.geocoders)
- [Nominatim](https://geopy.readthedocs.io/en/stable/#nominatim)

