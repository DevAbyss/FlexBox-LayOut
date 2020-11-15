### 1. FlexBox?

---

- viewport or element의 크기가 불명확하거나, 동적으로 변할 때에도 효율적으로 element를 배치, 정렬, 분산할 수 있는 방법을 제공하는 CSS3의 새로운 레이아웃 방식
- 복잡한 계산 없이 element의 크기와 순서를 유연하게 배치 가능
- 정렬, 방향, 순서, 크기 등을 유연하게 조절할 수 있기 때문에 별도의 분기 처리를 줄일 수 있고, CSS만으로 다양한 LayOut 구현 가능

### 2. FlexBox 구성

---

- FlexBox는 복수의 자식 element인 flex item과 그 상위 부모 element인 flex container로 구성
<div>
  <img width="500" src="https://user-images.githubusercontent.com/61103879/99178686-ff5fb600-2758-11eb-9e68-6f966facc834.png">
</div>

- 선언 방법

```css
.flex_container {
  display: flex;
}
```

- display: flex 속성이 적용된 element는 flex container가 되고, flex container의 자식 element는 flex item이 된다.

- flex item은 주축(main axis)에 따라 정렬
  주축의 방향은 flex container의 flex-direction 속성으로 결정
  flex-direction 속성을 따로 지정하지 않으면, 기본값인 row가 적용
  속성값 row는 주축의 방향을 왼쪽에서 오른쪽 방향으로 향함
  속성값 column은 주축의 방향을 위에서 아래 방향으로 향함

### 3. 부모 element와 자식 element에 정의하는 속성 구분

---

- FlexBox에서 사용하는 속성은 부모 element인 flex container에 정의하는 속성과 자식 element인 flex item에 정의하는 속성으로 나뉨
- 전체적인 정렬이나 흐름에 관련된 속성은 flex container에 정의하고, 자식 요소의 크기나 순서에 관련된 속성은 flex item에 정의 (분리해 적용하는 것이 중요!)

<div>
  <img width="500" src="https://user-images.githubusercontent.com/61103879/99180451-d4ca2900-2769-11eb-893b-94d331c5d9b0.png">
</div>
