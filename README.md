### Desc
이 페이지는 파이썬의 패키지, arisia에 대한 사용법을 다룹니다   
사용 중 문제가 발생하신다면 해당 페이지의 ISSUE를 통해서 안내해주세요   

___
[pypl] : https://pypi.org/project/arisia/   
<span style="color:pink">ARISIA pypl package address</span>

### 사용법 ( Usage )
1. 불러오기   
import arisia.load as al

2. 데이터 가져오기
<span style="color:tomato">print(<span style="color:beige">al.connect("예제 번호","타입")</span>)</span>   
데이터 형식 ("example"), 타입 : ("numpy","dataframe","df","np")   

3. 외부 데이터베이스 연결
print(al.connectdb("서버 주소", "포트 번호", "유저 아이디", "유저 비밀번호", "데이터베이스 이름", "타입", "쿼리"))   
[주의] 모든 파라미터에는 띄어쓰기가 없어야 합니다.   
[example] print(al.connectdb("test.com", 3306, "user", "password", "map", "np", "SELECT * FROM {table_name}"))   

4. 안내사항
모든 데이터는 넘파이 배열, 데이터프레임 두 가지 중 하나의 형식으로만 반환됩니다.   
추후 변경 사항은 업데이트를 참조하십시오.  
