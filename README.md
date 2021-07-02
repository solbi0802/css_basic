# basicOfCSS
CSS 기초적인 개념들 정리

### Selector
- 우선순위 : ID > Class(Pseudo-class도 포함) > Type

### Box
- box-sizing 
  - content-box : width,height 설정시, content영역의 크기로 지정됨. 따라서 w,h 지정해도 의도한 크기대로 나오지 않을 가능성이 있음.
  -  border-box : 별도 계산 없이 설정한 width, height로 적용됨

- Box Type (=display)
  #### Block 
    ![image](https://user-images.githubusercontent.com/26318691/124144843-48d1fb00-dac7-11eb-8df3-0ebc76446001.png)
    - 키워드 : 길막, 면
    
     ##### width
     따로 width를 선언하지 않은 경우, width = 부모의 content-box 의 100%
     따로 width를 선언한 경우, 남은 공간은 자동으로 margin으로 채움
    
     ##### height 특성
     따로 부모의 height를 선언하지 않을 경우, 자식 요소의 height의 합 = 부모의 height
    
     width,height,padding,border,margin box model에 있는 속성 모두 적용 가능

  #### Inline
    ![image](https://user-images.githubusercontent.com/26318691/124143917-7bc7bf00-dac6-11eb-9380-ba7ad977594f.png)
    - 키워드 : 흐름, 선
    - width,height,padding-top,padding-bottom, border-top,border-bottom,margin-top,margin-bottom 사용 못함 (Inline의 흐름을 방해하기 때문)

  #### Inline Block
  - Blcok && Inline : Inline과 Block의 특성을 둘 다 가지고 있음 

### Float
- inlineBlock,block -> block 으로 바뀜
- block의 특성인 width,height가 적용 되지 않고 자신의 content width,height만큼 자리를 차지하게 됨
- float를 사용할 경우 레이아웃이 틀어지게 된다
- 해결책 2가지 
  ##### overflow:hidden;
    ![image](https://user-images.githubusercontent.com/26318691/124336979-4d87d380-dbdb-11eb-92d2-76dbbc7c7f7c.png)
  ##### Clearfix
    ![image](https://user-images.githubusercontent.com/26318691/124337164-2b428580-dbdc-11eb-9e92-e530d79764b2.png)
    ![image](https://user-images.githubusercontent.com/26318691/124337246-92f8d080-dbdc-11eb-9d9b-13b4e2ba61a8.png) 
    ![image](https://user-images.githubusercontent.com/26318691/124337284-b02d9f00-dbdc-11eb-86e5-ad0001534c24.png)

