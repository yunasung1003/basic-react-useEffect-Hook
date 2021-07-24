컴포넌트 마운트: 나타난다.
컴포넌트 언마운트: 삭제된다.

useEffect 사용(마운트) : props -> state, Rest API, D3 Video.js ,setInterval, setTimeout
(언마운트): clearInterval, clearTimeout, 라이브러리 인스턴스


useEffect 의 첫번째 파라미터: 함수 등록
useEffect 의 두번째 파라미터: deps 배열 등록
retun: 어떤 특정 함수를 반환하면 뒷정리 함수이기 때문에, 업데이트 되기전 호출 된다.


  useEffect(( ) => {

    return() => {
   
    }
  }, [user]);

조회하고 있는 값 또는 프롭스가 있다면 예: [user] 라고 넣어줘야함.
1) ) => {

    }
  }, 
이부분은 컴포넌트가 처음 나타날 때만 호출, user 가 바뀔 때도 호출

2)
    return() => {
    
cleaner 함수(return) 은 use객체가 바뀌기 직전에도 호출, 컴포넌트가 사라지기 전에도 호출!



  useEffect(() => {

    }
  }, );
(return 이 없을 땐)컴포넌트가 나타날때에만 나타남.





  useEffect(() => {
     return ()=>{ }
  }, []);
(return 을 써서 어떤 함수를 넣었을때) 컴포넌트가 사라질때에만 컴포넌트가 호출.

