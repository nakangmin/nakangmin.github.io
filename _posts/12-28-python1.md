<!doctype html>
<html>
<head>
<meta charset='UTF-8'><meta name='viewport' content='width=device-width initial-scale=1'>
<title>python_01_12_28 (1).ipynb</title>
</head>
<body><p>{
  &quot;nbformat&quot;: 4,
  &quot;nbformat_minor&quot;: 0,
  &quot;metadata&quot;: {
    &quot;colab&quot;: {
      &quot;name&quot;: &quot;python_01_12_28.ipynb&quot;,
      &quot;provenance&quot;: [],
      &quot;collapsed_sections&quot;: []
    },
    &quot;kernelspec&quot;: {
      &quot;name&quot;: &quot;python3&quot;,
      &quot;display_name&quot;: &quot;Python 3&quot;
    },
    &quot;language_info&quot;: {
      &quot;name&quot;: &quot;python&quot;
    }
  },
  &quot;cells&quot;: [
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;# 파이썬 기본 문법\n&quot;,
        &quot;\n&quot;,
        &quot;## 목차\n&quot;,
        &quot;\n&quot;,
        &quot;1. 데이터 입력과 출력\n&quot;,
        &quot;2. 변수\n&quot;,
        &quot;3. 자료형\n&quot;,
        &quot;4. 문자열\n&quot;,
        &quot;  - 인덱스\n&quot;,
        &quot;  - 슬라이싱\n&quot;,
        &quot;5. 리스트\n&quot;,
        &quot;6. 딕셔너리\n&quot;,
        &quot;7. 연산자\n&quot;,
        &quot;8. 제어문\n&quot;,
        &quot;  - if\n&quot;,
        &quot;  - while\n&quot;,
        &quot;  - for\n&quot;,
        &quot;9. 함수\n&quot;,
        &quot;\n&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;HcNCOed9YNLN&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 1. 문자열 표현\n&quot;,
        &quot;\n&quot;,
        &quot;- 따옴표로 둘러싸면 모두 문자열\n&quot;,
        &quot;\n&quot;,
        &quot;- 함수 print(출력될 자료)\n&quot;,
        &quot;\n&quot;,
        &quot;  -문자열이나 숫자 등의 자료를 콘솔에 출력하는 일을 수행\n&quot;,
        &quot;\n&quot;,
        &quot;  -출력 이후에 다음 줄로 이동해 출력을 준비&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;cyZu4qtvY2wY&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;&#39;p&#39;\n&quot;,
        &quot;\n&quot;,
        &quot;&quot;python&quot;\n&quot;,
        &quot;\n&quot;,
        &quot;&quot;4.15&quot;\n&quot;,
        &quot;\n&quot;,
        &quot;print(&quot;Hello world!&quot;)\n&quot;,
        &quot;print(&#39;Hello python&#39;)&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;
        },
        &quot;id&quot;: &quot;_N7PpoupZP7i&quot;,
        &quot;outputId&quot;: &quot;e4a99d9a-6ccb-4e1e-95af-0d43a6b54ac0&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;stream&quot;,
          &quot;name&quot;: &quot;stdout&quot;,
          &quot;text&quot;: [
            &quot;Hello world!\n&quot;,
            &quot;Hello python\n&quot;
          ]
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 2. 자료형과 type() 함수\n&quot;,
        &quot;\n&quot;,
        &quot;- 자료형 :정수와 실수, 문자열 등\n&quot;,
        &quot;\n&quot;,
        &quot;- type() 함수\n&quot;,
        &quot;\n&quot;,
        &quot;  -자료형 이름 출력\n&quot;,
        &quot;\n&quot;,
        &quot;  -자료형을 직접 알아보는 방법&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;i6HUNYNYaY1b&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;type(3) #int\n&quot;,
        &quot;\n&quot;,
        &quot;pi = 3.14\n&quot;,
        &quot;type(pi) #float\n&quot;,
        &quot;\n&quot;,
        &quot;type(&#39;python&#39;) # str\n&quot;,
        &quot;\n&quot;,
        &quot;type(3 + 4j) # complex = 복소수는 class complex 클래스\n&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;
        },
        &quot;id&quot;: &quot;TLbZPgBhbrgQ&quot;,
        &quot;outputId&quot;: &quot;f9cc723e-e157-4ad6-b2c9-3b7a58bdef6d&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;text/plain&quot;: [
              &quot;complex&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 8
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 3. 변수와 대입 연산자\n&quot;,
        &quot;\n&quot;,
        &quot;- 변수(variavle) : &#39;변하는 자료를 저장하는 메모리 공간&#39;\n&quot;,
        &quot;\n&quot;,
        &quot;  - 변수는 자료를 담을 수 있는 그릇\n&quot;,
        &quot;\n&quot;,
        &quot;  - 그릇에 이름인 태그가 붙어 있다고 생각\n&quot;,
        &quot;\n&quot;,
        &quot;- 대입 연산자(=)\n&quot;,
        &quot;\n&quot;,
        &quot;  - 값을 변수에 저장, =의 의미는 왼쪽 화살표(&lt;-)라고 생각\n&quot;,
        &quot;\n&quot;,
        &quot;- 식별자(identifiers)\n&quot;,
        &quot;  - 변수, 함수와 클래스 이름 등 프로그래머가 이름을 짓는 단어\n&quot;,
        &quot;  - 식별자를 구성하는 문자 (영문자, 한글도 가능와 숫자 그리고 _를 사용)\n&quot;,
        &quot;- 제한\n&quot;,
        &quot;  - 문자는 대소문자의 영문자,숫자 그리고 _구성\n&quot;,
        &quot;  - 대소문자는 구별\n&quot;,
        &quot;  - 숫자는 맨 앞에 올 수 없다\n&quot;,
        &quot;  - 키워드는 불가\n&quot;,
        &quot;\n&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;s3mLJcvveCcI&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;unit = 3 # true\n&quot;,
        &quot;# 3 = unit error\n&quot;,
        &quot;\n&quot;,
        &quot;5 == 3 + 2 # 등호식의 &#39;같다&#39;라는 등호 연산자 ==으로, 결과는 true 또는 false다.&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;
        },
        &quot;id&quot;: &quot;jQ9mv2ANeroK&quot;,
        &quot;outputId&quot;: &quot;6d5ac440-0185-46da-987c-21e0258bd1e9&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;text/plain&quot;: [
              &quot;True&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 11
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 4. 표준 입력의 이해\n&quot;,
        &quot;\n&quot;,
        &quot;- 표준 입력(standard input)\n&quot;,
        &quot;  - 쉘이나 콘솔에서 사용자의 입력을 받아 처리하는 방식\n&quot;,
        &quot;  - 콘솔의 키보드로 입력되는 방식을 표준 입력\n&quot;,
        &quot;  - 모니터의 콘솔로 출력되는 방식을 표준 출력\n&quot;,
        &quot;- 함수 input()  사용\n&quot;,
        &quot;  - 함수 input(&#39;질문 내용?&#39;)\n&quot;,
        &quot;  -Enter 키를 누르기 전에 입력한 한 줄의 모든 내용이 문자열로 반환&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;zq4y6bKzfGxU&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;univ = input(&#39;대학은? &#39;) # 대학은? <strong>_enter\n&quot;,
        &quot;name = input(&#39;이름은? &#39;) # 이름은? _</strong>enter\n&quot;,
        &quot;print(&#39;대학 : &#39;,univ, &#39;이름 : &#39;, name)\n&quot;,
        &quot;\n&quot;,
        &quot;d = input() # 문자열로 받기 때문에 형변환을 해야한다\n&quot;,
        &quot;int(d) + 5\n&quot;,
        &quot;\n&quot;,
        &quot;data = int(input()) #input에다가 int로받아라\n&quot;,
        &quot;type(data)&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;
        },
        &quot;id&quot;: &quot;x1mW32L3gYcx&quot;,
        &quot;outputId&quot;: &quot;feafc5ca-56c1-4066-917c-ace321615c05&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;name&quot;: &quot;stdout&quot;,
          &quot;output_type&quot;: &quot;stream&quot;,
          &quot;text&quot;: [
            &quot;대학은? tjdnfeo\n&quot;,
            &quot;이름은? 나강민\n&quot;,
            &quot;대학 :  tjdnfeo 이름 :  나강민\n&quot;,
            &quot;100\n&quot;,
            &quot;423\n&quot;
          ]
        },
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;text/plain&quot;: [
              &quot;int&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 18
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 5. 문자열 활용, 길이와 문자 참조\n&quot;,
        &quot;  - 문자열의 길이 반환 : 함수 len()\n&quot;,
        &quot;  - 첨자를 사용한 문자열의 문자 참조&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;6arydkMXgttm&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;str = &#39;Hello python!&#39;\n&quot;,
        &quot;n = len(str)\n&quot;,
        &quot;print(&#39;문자열&#39;, str, &#39;길이&#39;, n)\n&quot;,
        &quot;print(&#39;첫 문자&#39;, str[0], str[-n])\n&quot;,
        &quot;print(&#39;가운데 문자&#39;, str[n//2], str[-n//2])\n&quot;,
        &quot;print(&#39;마지막 문자&#39;, str[n-1], str[-1])&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;
        },
        &quot;id&quot;: &quot;8_IzR0Poikm3&quot;,
        &quot;outputId&quot;: &quot;48a2ee2c-2a72-4167-8c52-1868ac21614e&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;stream&quot;,
          &quot;name&quot;: &quot;stdout&quot;,
          &quot;text&quot;: [
            &quot;문자열 Hello python! 길이 13\n&quot;,
            &quot;첫 문자 H H\n&quot;,
            &quot;가운데 문자 p p\n&quot;,
            &quot;마지막 문자 ! !\n&quot;
          ]
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 6. 슬라이싱 : 문자열의 부분 문자열 참조 방식\n&quot;,
        &quot;\n&quot;,
        &quot;- 슬라이싱(slicing)\n&quot;,
        &quot;  - 전체에서 일부분을 참조하는 방법\n&quot;,
        &quot;- 문자열 슬라이싱\n&quot;,
        &quot;  - 기존의 문자열은 절대 수정이 되는 것이 아니라 원 문자열은 변함이 없고 일부분을 반환\n&quot;,
        &quot;- str[start : end]\n&quot;,
        &quot;  - 문자열 str에서 start 첨자에서 end - 1 첨자까지의 문자열을 반환&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;kNhDC6ENjKDT&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;&#39;python&#39;[1:5] #ytho\n&quot;,
        &quot;&#39;python&#39;[2:4] #th\n&quot;,
        &quot;&#39;python&#39;[0:3] #pyt\n&quot;,
        &quot;&#39;python&#39;[0:6] #python\n&quot;,
        &quot;&#39;python&#39;[0:len(&#39;python&#39;)] #python&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;,
          &quot;height&quot;: 35
        },
        &quot;id&quot;: &quot;-fJehARoj54M&quot;,
        &quot;outputId&quot;: &quot;f7cf7521-6d8f-4524-fbdf-6d8888cf7bb1&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;application/vnd.google.colaboratory.intrinsic+json&quot;: {
              &quot;type&quot;: &quot;string&quot;
            },
            &quot;text/plain&quot;: [
              &quot;&#39;python&#39;&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 16
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 7. 함수 count()와 join()\n&quot;,
        &quot;\n&quot;,
        &quot;- 메소드 count() : 부분 문자열 출현 횟수를 반환\n&quot;,
        &quot;- 메소드 join() : 문자열의 문자와 문자 사이에 원하는 문자열을 삽입\n&quot;,
        &quot;\n&quot;,
        &quot;- 함수는 독립적으로 직접 호출하지만 메소드는 객체를 통해 호출한다.\n&quot;,
        &quot;  - 함수(function) : len(&#39;python&#39;) 독립적\n&quot;,
        &quot;  - 메소드(method) : &#39;python&#39;.count(&#39;th&#39;) 객체 또는 클래스에 소속&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;hwMe2JDjlclh&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;str = &#39;단수한 것이 복잡한 것보다 낫다.&#39;\n&quot;,
        &quot;str.count(&#39;복잡&#39;) # 1\n&quot;,
        &quot;str.count(&#39;것&#39;) # 2\n&quot;,
        &quot;\n&quot;,
        &quot;num = &#39;12345&#39;\n&quot;,
        &quot;&#39;-&gt;&#39;.join(num) # 1-&gt;2-&gt;3-&gt;4-&gt;5&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;,
          &quot;height&quot;: 35
        },
        &quot;id&quot;: &quot;-g7xtPtolzBI&quot;,
        &quot;outputId&quot;: &quot;fc561c3e-1620-4600-eac4-d903aa882240&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;application/vnd.google.colaboratory.intrinsic+json&quot;: {
              &quot;type&quot;: &quot;string&quot;
            },
            &quot;text/plain&quot;: [
              &quot;&#39;1-&gt;2-&gt;3-&gt;4-&gt;5&#39;&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 20
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 8. C언어의 포맷팅 스타일인 %d와 %f 등으로 출력\n&quot;,
        &quot;\n&quot;,
        &quot;- %d, %x, %o, %f, %c, %s 등을 사용해 %로 이어지는 뒤의 상수나 변수를 순서대로 10진수, 16진수, 8진수, 소수점, 문자, 문자열로 출력&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;SOH9edWNmKwz&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;code&quot;,
      &quot;source&quot;: [
        &quot;&#39;%d - %x = %o&#39; % (30, 20, 30-20) #30 - 14 = 12\n&quot;,
        &quot;print(&#39;%d ** %x = %o&#39; % (3, 2, 3<strong>2)) #3 </strong> 2 = 11\n&quot;,
        &quot;print(&#39;%10.2f&#39; % 2.7124782) #      2.71\n&quot;,
        &quot;x = 70\n&quot;,
        &quot;y = 120\n&quot;,
        &quot;&#39;%d + %d = %d&#39; % (x, y, x+y) # 70 + 120 = 190&quot;
      ],
      &quot;metadata&quot;: {
        &quot;colab&quot;: {
          &quot;base_uri&quot;: &quot;<a href='https://localhost:8080/' target='_blank' class='url'>https://localhost:8080/</a>&quot;,
          &quot;height&quot;: 72
        },
        &quot;id&quot;: &quot;yDNQTUUKnadS&quot;,
        &quot;outputId&quot;: &quot;410891be-1365-4540-d9b8-c0ccb036f561&quot;
      },
      &quot;execution_count&quot;: null,
      &quot;outputs&quot;: [
        {
          &quot;output_type&quot;: &quot;stream&quot;,
          &quot;name&quot;: &quot;stdout&quot;,
          &quot;text&quot;: [
            &quot;3 ** 2 = 11\n&quot;,
            &quot;      2.71\n&quot;
          ]
        },
        {
          &quot;output_type&quot;: &quot;execute_result&quot;,
          &quot;data&quot;: {
            &quot;application/vnd.google.colaboratory.intrinsic+json&quot;: {
              &quot;type&quot;: &quot;string&quot;
            },
            &quot;text/plain&quot;: [
              &quot;&#39;70 + 120 = 190&#39;&quot;
            ]
          },
          &quot;metadata&quot;: {},
          &quot;execution_count&quot;: 25
        }
      ]
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;## 8. 내장 함수 정리하기!&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;c-Sl2Yrlpj4n&quot;
      }
    },
    {
      &quot;cell_type&quot;: &quot;markdown&quot;,
      &quot;source&quot;: [
        &quot;### 파이썬 자습서 : python Tutorial(파이썬 자습서) 검색\n&quot;,
        &quot;\n&quot;,
        &quot;<a href='https://docs.python.org/ko/3/tutorial/index.html' target='_blank' class='url'>https://docs.python.org/ko/3/tutorial/index.html</a>\n&quot;,
        &quot;\n&quot;,
        &quot;기본적인건 정리 했지만 라이브러리 함수들을 좀 더 공부해야한다.&quot;
      ],
      &quot;metadata&quot;: {
        &quot;id&quot;: &quot;Me88NQJxohR4&quot;
      }
    }
  ]
}</p>
</body>
</html>