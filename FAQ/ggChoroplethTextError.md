ggChoropleth()로 만든 단계 구분도의 한글이 깨질 때
-----------------------------------------------------

윈도우 사용자의 경우 `iconv()`를 이용해 `name`의 인코딩을 `CP949`로 바꾼 다음 단계 구분도를 생성하면 한글이 정상적으로 출력됩니다.

`korpop1$name <- iconv(korpop1$name, "UTF-8", "CP949")`