Clumsy Smelting
===

요약
---
금속 제련이 조금 더 복잡해졌습니다.

Furnace
---
Furnace는 마인크래프트 내에서 2가지 용도가 있습니다.

1. 음식의 조리
2. 광물의 제련

이 중, 음식의 조리의 경우 훈연기에서 속도가 더 빨라지며, 제련의 경우 용광로에서 속도가 더 빨라집니다.
여기에서는 광물의 제련에 더 초점을 맞추려고 합니다.

철의 제련
---
물론 현실의 제련 과정을 완벽히 모방하는 것은 불가능하고, 어느 정도의 게임적 허용이 있을 수밖에 없습니다.
그러나 본 플러그인에서는 제련 과정을 조금이라도 더 자세히 나누는 것에 초점을 맞춥니다.
[철의 제련](https://dic.kumsung.co.kr/web/smart/detail.do?headwordId=1917&findCategory=B002004&findBookId=26) 
에는 철광석과 코크스(환원제), 석회석(용제)가 필요합니다.
그런데, 마인크래프트에는 코크스와 석회석이 존재하지 않습니다.
본 플러그인에서는, 아쉽게도 석회석은 구현하지 못하였고 코크스만을 구현했습니다.

코크스
---
현대 철의 제련에 환원제로 사용되는 재료입니다. 코크스는 석탄을 
[건류](https://www.scienceall.com/%EC%84%9D%ED%83%84%EA%B1%B4%EB%A5%98-coal-carbonization/)
하여 만들 수 있습니다.
따라서, 본 플러그인에서 코크스의 획득 방법은 2가지입니다.

1. 석탄 건류 : 화로 혹은 용광로를 사용하여 석탄을 가열하면, 코크스가 나옵니다.
2. 자연 채광 : 희귀하지만, 
[자연 상태](https://ko.wikipedia.org/wiki/%EA%B3%A0%EC%B2%B4%EC%97%B0%EB%A3%8C#%EC%BD%94%ED%81%AC%EC%8A%A4)
에도 코크스가 존재한다고 합니다.
따라서, 석탄 광석을 채광하면, 낮은 확률(기본 5%)로 코크스가 드랍됩니다.

코크스의 형태는 석탄과 같으며, 이름은 Coke로 표기되어 있습니다.
원래 코크스는 석탄과 연료 효과가 차이가 있을 테지만, 여기서는 석탄과 코크스의 연료 효과가 같습니다.

선철
---
바닐라 마인크래프트와 같이 화로에서 철광석을 제련하면 선철을 얻을 수 있습니다. 
이때, 손에(왼손, 오른손 상관 없음) 코크스를 들고 있다면, 불순물 함량이 낮은 선철을, 들고 있지 않다면 높은 선철을 얻습니다.
용광로에서 철광석을 제련할 경우, 불순물 함량이 낮은 선철을 확정적으로 얻습니다.
선철은 다른 철괴를 제조하는데 사용되는 선행 재료입니다.

주철
---
본래 주철은 탄소 함량이 높고 주조법으로 만든 철을 의미합니다.
주조법으로 만들기 때문에 원래는 만들고 싶은 모양대로 만들 수 있습니다.
그러나, 본 플러그인에서는 주철의 본래 제련법 대신에 다른 방식을 도입했습니다.
대장장이 작업대에서 도구 칸에 화분을 놓고(주형), 네더라이트 칸에 선철을 놓으면 주철을 얻을 수 있습니다.
주철의 불순물 함량은 재료로 사용 된 선철의 불순물 함량과 같습니다.

강철
---
본래 강철은 특별한 제강법을 통해 선철에서 얻을 수 있습니다.
따라서, 본 플러그인에서는 제강법에서 전로를 사용한다는 개념을 차용했습니다.
하급 전로(전로 품질이 10 이하)를 사용할 경우, 질 나쁜 강철이 나옵니다.
고급 전로(전로 품질이 10 초과)를 사용할 경우, 질 좋은 강철이 나옵니다.
그러나, 이 방식으로 얻을 수 있는 강철의 최대 품질은 1입니다.

수리 제한
---
인벤토리에서 수리하는 것이 금지됩니다.

용광로 변경
---
기존 용광로 조합법으로는 조합할 수 없습니다.
품질이 1 이상인 강철 5개, 화로, 석탈 블록 2개, 코크스 1개가 있어야 조합할 수 있습니다.

모루 변경
---
기존 모루 조합법으로는 조합할 수 없습니다.
품질이 18인 철블록 3개, (주철 또는 강철) 4개가 있어야 조합할 수 있습니다.

품질
---
철을 이용하여 제작 가능한 도구는 품질이라는 새로운 특성을 갖습니다.

강철 태그
---
철을 이용하여 제작 가능한 도구는 강철이라는 특성을 가질 수 있습니다.
조합할 때 강철이 최소 1개 이상 들어갔다면, 금색으로 강철 태그가 붙습니다.
조합할 때 사용한 모든 철이 강철이었다면, 노란색으로 강철 태그가 붙습니다.
사용한 모든 철이 강철이었을 때, 품질이 2인 강철이 최소 1개 이상 사용되었다면, 강철+ 태그가 붙습니다.
사용한 모든 철이 품질이 2인 강철이었다면, 강철++ 태그가 붙습니다.
강철 태그가 붙을 경우, 몇몇 아이템은 특수한 효과를 받습니다.