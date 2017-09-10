디자인 패턴 : MVC 패턴
====================================================================

### 디자인패턴

> [_디자인 패턴_]()이란 프로그램 개발에서 자주 나타나는 과제를 해결하기 위한 방법 중 하나로, 과거의 소프트웨어 개발 과정에서 발견된 설계의 노하우를 축적하여 이름을 붙여, 이후에 재이용하기 좋은 형태로 특정의 규약을 묶어서 정리한 것이다. 알고리즘과 같이 프로그램 코드로 바로 변환될 수 있는 형태는 아니지만, 특정한 상황에서 구조적인 문제를 해결하는 방식을 설명해 준다.

### MVC 패턴

  1. MVC란?

  > __MVC__ 란 Model-View-Controller의 약자로 어플리케이션을 세가지의 역할로 구분한 소프트웨어 디자인 패턴 중 하나이다. 주로 웹개발에서 많이 사용되며 이 패턴을 성공적으로 사용하면, UI와 비즈니스 로직이 서로 영향 없이 쉽게 변경이 가능하다. ([위키피디아](https://ko.wikipedia.org/wiki/%EB%AA%A8%EB%8D%B8-%EB%B7%B0-%EC%BB%A8%ED%8A%B8%EB%A1%A4%EB%9F%AC, [생활코딩](https://opentutorials.org/course/697/3828))

    - Model

        - Data의 전반적인 부분과 처리를 담당한다. 네트워크, 로컬 데이터 등을 포함한다.

    - View

        - UI(화면)를 담당한다. 사용자가 볼 결과물을 생성하기 위해 Model 에 요청한다.

    - Controller

        - 비즈니스 로직을 담당한다. 사용자의 요구사항에 맞는 데이터를 Model 에 요청하고, 그 데이터를 View에 반영하여 사용자에게 알려준다.

  2. MVC 흐름도

        ![MVC 흐름도](https://github.com/Hooooong/DAY4_MVC/blob/master/image/MVC.PNG)

        1. 사용자가 요청을 하면, `Controller` 는 그 요청에 맞는 데이터를 `Model` 에 요청한다.
        2. `Model` 은 요청한 데이터를 `Controller`에 전달하고,
        3. `Controller`는 데이터를 `View` 에 전달한다.
        4. `View`는 그 데이터에 맞게 화면을 구성하고,
        5. 사용자에게 `View` 를 전달한다.
