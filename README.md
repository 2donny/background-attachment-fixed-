# background-attachment-fixed-
background-attachment의 속성의 값을 fixed 라고 지정했을 때, 스크롤을 내림에 따라서 background image가 어떻게 보이는지 살펴본다.

background-size가 이해하기 가장 어려웠습니다.
간단하게 설명을 해보겠습니다.

우리는 이미지를 section이라는 요소 안에 보통 삽입합니다. 그리고 그 요소의 부모 요소를 통해 또 그것을 래핑하죠.
먼저 자식 요소(section1)의 css에 가서 background-image:url('https://www.~~~');를 통해서 배경 이미지를 가져옵니다.

background-size: 100%를 입력한다면, 부모요소의 모든 크기를 활용해서 이미지를 가져온다는 뜻입니다. 
만약 section1 요소의 크기가 background 이미지의 크기보다 작다면 잘릴것입니다. 왜냐하면 요소의 크기를 100% 활용하기 때문입니다.
근데 요소에 이미지를 삽입할 때, 이미지의 왼쪽 위에서부터 요소에 넣기 시작하기 떄문에, 상대적으로 right bottom에 있는 이미지는 짤립니다.

위 html, css 코드는 스타벅스 웹페이지에서 제공되는 html 문서를 참고하여 클론해보았습니다.

어렵지만 유용한 코드입니다 ^^

