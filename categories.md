---
layout: page
title: Python
header: Posts By Category
group: navigation
---



#0@ Variables
##### how to store data in Python


---

##목차
<a href = "#C1">1. 변수에 관하여</a>
<br><br><a href = "#C2">2. 변수와 사용 가능한 값의 종류   </a>
<br><br><a href = "#C3">3. 변수 사용상의 유의사항</a>
<br><br><a href = "#Ref">참고 사이트 / 문헌 목록</a>
<br><br><a href = "#Do">직접 해 봅시다. </a>
<br><br><a href = "#Sum">요약					</a>
<br><br><a href = "#Rep">댓글					</a>




---

<a name = "C1">1 . 변수에 관하여</a>
<br>
<br>변수라는 건 프로그램 내에서 나중에 사용하기 위해 특정 값을 저장해두는 것을 의미합니다.<br><br>
단순한 수는 물론, 실수나 복소수, 문장과 같은 글자를 저장하는 경우에도 해당합니다.
<br><br>이 값의 저장 방식으로 파이썬에서는 레퍼런스 방식을 사용합니다.
<br><br> 이름을 가진 변수와 그 변수에 연결된, 지정된 값을 가지는 레퍼런스를 만들어서 놓아두는 형식이죠.<br><br> 레퍼런스라는 말이 어려우신 분은 '참조값' 같은 정도로 이해하시면 될 겁니다.

중간 점검: '레퍼런스' 라는 개념을 지금 무리해서 이해할 필요는 없습니다. <br><br> 우선 '변수' 라는 게 우리가 저장하고 싶은 특정 값을 저장할 때 사용하는 것이라는 점만 알고 넘어갑시다.

변수를 만드는 방법은 왼쪽엔 변수의 이름에 해당하는 부분을, 오른쪽에는 그 이름에 연결해 줄 값을 쓰고 대입한다는 의미로 = 기호를 사용합니다. 보통 이런 과정을 변수에 그 값을 저장한다고 표현합니다. 정확하게는 그렇지 않더라도 알기 쉽게 축약해서 표현하는 것이죠.
<br><br>//이곳에 이미지를 넣는다. a를 만들고 -> 1이라는 값이 등장하고 -> 연결하는 이미지.
//Python Tutor의 기능을 적당하게 활용하자.
<br><br>가령, a라는 이름을 가진 변수에 1이라는 수의 값을 저장하려면 a=1이라고 표현합니다.
<br><br>즉석에서 무언가 계산을 해서 그 결과를 저장할 수도 있습니다. b = 10+5라고 쓰면 b에 15의 값을 바로 저장하는 효과를 가집니다.
<br><br>(이 계산에 대한 자세한 이야기는 다음 챕터, 기본적인 연산 쪽에서 다루도록 하겠습니다.)
<br><br>변수의 이름이라는 건 그 자체가 다른 것과 구별되는 지칭 방식을 이야기합니다만, 몇 가지 정도의 제약 조건은 있습니다. <br><br>자세한 내용은 이번 장의 제 3파트, <a href = "#C3">유의사항 항목을 참조하세요.</a>

[파이썬 3 계통에선 변수 이름으로 한글을 지원합니다...란 내용 넣어야 하나 말아야 하나.]

중간 점검 : 아무튼 변수는 <span title = "변수명">**_그 고유의 이름</soan>_**과 <span title = "레퍼런스 위치의 값">**_그것에 연결되는 값_**</span>으로 이루어져 있다는 것, <br><br>그리고 그 값을 지정하기 위해 등호를 사용한다는 것만 알고 넘어갑시다.

//리터럴에 대한 것은 나중에 언젠가 다루기로 합니다.

---

<a name = "C2">2 . 변수와 사용 가능한 값의 종류</a>
<br><br>파이썬에선 상당히 다양한 종류의 값을 간단한 형태로 저장하여 사용하는 것이 가능합니다.
<br><br>아래의 다양한 예시를 보면서 사용 가능한 값에 무엇이 있는지 확인해 봅시다.

<table class="tg">
  <tr>
    <th class="tg-99b9">값의종류</th>
    <th class="tg-99b9">값의 예시</th>
  </tr>
  <tr>
    <td class="tg-99b9">int(정수)</td>
    <td class="tg-99b9">1, 2, 3, 4, ......</td>
  </tr>
  <tr>
    <td class="tg-99b9">float(실수)</td>
    <td class="tg-99b9">1.0, 2.5, 3.7, .......</td>
  </tr>
  <tr>
    <td class="tg-99b9">str(문자열)</td>
    <td class="tg-99b9">'Hello', 'Python', ....</td>
  </tr>
  <tr>
    <td class="tg-99b9">char(문자)</td>
    <td class="tg-99b9">"c", "w", "a", .....</td>
  </tr>
  <tr>
    <td class="tg-99b9">Long(큰정수)</td>
    <td class="tg-99b9">99999999999, ....</td>
  </tr>
</table>
**복소수의 경우 i가 아니라 j를 사용하는 것에 주의합시다.**
<br><br>~~i를 쓰면 대문자일 때 L의 소문자와 구분이 어려워서 그러는 게 아닐까 싶습니다.~~<br><br>
정확한 이유는 j를 쓰는 편이 보다 벡터 표현을 복소 평면으로 옮길 때 자연스러워서 그런 거라고 합니다.<br><br>
다만 쓸데없이 복잡하게 설명이 들어가 있고, 웬만하면 복소수 쓸 일 없으니 그냥 J인가 보다 하세요. 

---

<a name = "C3">3 . 변수 사용상의 유의사항</a>

1. <p>중복해서 값을 저장하려 하면 이전 값이 사라진다는 점.
a에 1이란 값을 넣었다가 2라는 값을 넣은 뒤 print 해준다.
</p>

2. 한 변수에 정해진 형태가 없다는 점
그 외에 다양한 자료 형을 넣으면서 이런 게 되니까 잘 모르고 쓰면 위험하다는 사실을 보여주고 설명을 적어 준다.<br><br>
다시 말해 실수로 엉뚱한 값을 넣을 수도 있다는 것.

3. 오버플로우 관련 이야기.
수를 억 정도 되는 값을 계속 더해가며 출력해본다.//21억 기준으로 될 것도 같은데 롱으로 바뀌면 어떡하짘ㅋㅋㅋ 일단 해보고 생각합시다.

4. 이름 작명 관련 이야기.
이름 관련 주의사항은 여기에 기록한다.
//교재를 참고해보자.

5. 기타 고민해보자... 'ㅅ'/

---


<a name = "Sum">요약</a>

내용을 채우자....

---

<a name = "Ref">참고 사이트 / 문헌 목록</a>

내용을 채우자....

1. Codeacademy.com
2. Let's learn Python programming
3. Python Tutor....넣을 수 있으면 좋겠지만.

---


<a name = "Do">직접 해 봅시다.</a>

//실습 공간 만들기 - python tutor를 사용할 수 있다면 여기에 넣도록
//안 된다면? 웹 IDLE의 링크를 걸어 주자.


---

<a name = "Rep">댓글 달기</a>




<form id="contact-form" action="script.php" method="post">
  <fieldset>
    <legend>Contact Us:</legend>    <ul>
      <li>        <label for="name">Name:</label>
        <input type="text" name="name" id="name" value="" />
      </li>
      <li>        <label for="email">Email:</label>
        <input type="text" name="email" id="email" value="" />
      </li>
      <li>        <label for="comments">Comments:</label>
        <textarea name="comments" id="comments" cols="25" rows="3"></textarea>
      </li>
      <li>        <label for="mailing-list">Would you like to sign up for our mailing list?</label>
        <input type="checkbox" checked="checked" id="mailing-list" value="Yes, sign me up!" />
      </li>
      <li>        <input type="submit" value="submit" />        <input type="reset" value="reset" />
      </li>
    </ul>
  </fieldset>
</form>

{% include JB/setup %}

<ul class="tag_box inline">
  {% assign categories_list = site.categories %}
  {% include JB/categories_list %}
</ul>


{% for category in site.categories %} 
  <h2 id="{{ category[0] }}-ref">{{ category[0] | join: "/" }}</h2>
  <ul>
    {% assign pages_list = category[1] %}  
    {% include JB/pages_list %}
  </ul>
{% endfor %}

