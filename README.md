![header](https://capsule-render.vercel.app/api?height=200&type=waving&text=UI_Practice!&animation=fadeIn&fontAlign=70)

## first_chall
<img width="302" alt="image" src="https://github.com/hyunwookoo13/Nomad_UI/assets/97423451/94371af0-ff63-4f18-8a05-999629e51b60">

1. Row/Column/padding/mainAxisAlignment/crossAxisAlignment 사용
2. Transfer/Request 버튼 커스터마이징해서 사용하기
3. Card 3개 커스터 마이징해서 사용하기
    - Transform.scale() + Transform.translate() + Offset으로 아이콘이 overflow하게 사이즈가 커지지만 container 밖으로 나가지 않도록 구현.
<br>
<h2>Second_chall</h2>
<img width="302" alt="image" src="https://github.com/hyunwookoo13/Nomad_UI/assets/97423451/0f773232-b8ec-42dd-80c1-1ac530c3bcfb">

1. MaterialApp()에서 Theme을 정해주었다. 
    - colorScheme : backgroundColor
    - textTheme : text
    - cardColor : card
2. Flexible() 사용
    - flex: UI를 비율에 기반해서 더 유연하게 공간을 사용할 수 있게 된다. 
    - Container() : alignment: Alignment.bottomCenter로 정렬 가능.
        - decoration: 컨테이너의 color, borderRadius 등에 변화를 주었다. 
3. 함수와 지역변수 & Timer 사용
    - setState()로 상태 변화를 줬다.
    - static const로 변하지 않는 값은 지정해주는 것이 좋다.
    - late Timer timer: late로 나중에 값을 넣어준다 하고 선언만 해줬다. 
    - bool isRunning으로 true할 때 변화하고, false일때 타이머가 멈추도록 했다. 
    - onTick(), onStartPressed(), onPausePressed()로 타이머를 움직였다. 
    - String format(int seconds)
        - Duration(seconds: seconds)을 사용해서 1500초를 25:00로 표현하고 싶었다. 
        - duration.toString().split(".").first.substring(2,7)
            - split()와 substring()으로 이를 표현해주었다. 
