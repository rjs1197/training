## Introduction  

##### Flask framework에 대한 배경과 장점, 특징에 대해 살펴보자.  

[뒤로가기](/web/flask/README.md)

### Flask Web Framework  

플라스크는 표준을 따르는 아주 작은 규모의 '마이크로프레임워크'이다. 물론, 작다고 해서 다른 프레임워크에 비해 성능이 떨어지는 것은 아니니 안심하도록 하자.  

플라스크의 가장 큰 장점이자 특징은 기본 서비스를 제공하는 코어를 필수적으로 구성하게끔 만들어졌고, 나머지 기능은 확장(extension)의 개념으로 제공하는 것이다.  

> 그렇기 때문에 원하는 확장 패키지를 선택해 만들고자 하는 기능을 손쉽게 구현할 수 있다.  

### Flask의 두 가지 의존성  

여기서의 의존성은 다른 프로젝트에 의존해 사용하는 기능 때문에 발생한다. 웹 서버 게이트워에 인터페이스(Web Server Gateway Interface, WSGI) 서브시스템, 라우팅(Routing) 그리고 디버깅(Debuging)의 기능은 Werkzeug에 의존하고, 템플릿에 대한 지원은 Jinja2 Engin에 의존한다.  

이 둘에 대한 자세한 설명은 여기서 다루지 않지만, 보다 심화적인 내용이 궁금하다면 다음 링크를 참고하도록 하자.  

- [Jinja2 Docs1](http://www.alexkrupp.com/Jinja%20docs.html)
- [Jinja2 Docs2](http://jinja.pocoo.org/docs/)
- [Werkzeug Docs](http://werkzeug.pocoo.org/docs/)

### Flask의 특징  

플라스크에서는 DB를 엑세스하고 웹 폼을 검증하거나 사용자를 인증하는 등의 기능을 기본적으로 지원하지 않는다.  

이러한 기능들이 기본적으로 제공되지 않기 때문에 앞서 언급했던 확장(extensions)을 통해 웹 애플리케이션에 필요한 많은 서비스를 사용해야 하는 것이다.  

이러한 특징은 개발자가 자신의 프로젝트에 적합한 확장을 선택하여 의도하는 기능을 작성하는 등 유연성을 보장한다는 장점이 있고, 다른 큰 규모의 프레임워크들과는 상반된 구조를 지닌다.  

> 다른 대규모 프레임워크들은 기본적으로 많은 서비스를 제공하고, 사용자는 많은 서비스중에 하나를 선택하거나 서비스가 구현된 그대로 사용해야 하기 때문에 상대적으로 유연하지 못하다.  




