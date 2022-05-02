## Set
---
###  중복값을 저장하지않는 정렬되지 않은 데이터

### 선언    
``` java     
		HashSet hs = new HashSet();
```		
### 출력
---
이터레이터로 변환해 출력
``` java
		Iterator<String> iter = hs.iterator();
		
		while(iter.hasNext()) {
			System.out.print(iter.next() + " ");
		}
```
### 정렬
---		
리스트로 형 변환후 정렬 가능
``` java		
		List arrList = new ArrayList(hs);
		Collections.sort(arrList);
		
		for(int i=0; i<arrList.size(); i++) {
			System.out.print(arrList.get(i)+ " ");
		}
```

### LIST VS SET 
---
LIST 로 출력시
``` java
3
1 3 5
5
2 3 6 7 9
1 2 3 3 5 6 7 9 
```
---
SET 으로 출력시
``` java
3
1 3 5
5
2 3 6 7 9
1 2 3 5 6 7 9 
```