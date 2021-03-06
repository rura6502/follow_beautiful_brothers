# Order(주문 시스템)

* 하나의 주문은 한 가게에서만 이루어 진다.
* 주문 정보에는 다음과 같은 정보를 포함한다.
  * 결제 품목
  * 결제 품목 당 수량과 가격
  * 포인트 사용 금액
  * 포인트 적립 금액 : (총 금액 - 포인트 사용 금액) x 가게 포인트 적립률
  * 최종 가격
  * 배송지
  * 배송상태
  * 주문상태
* 결제가 완료되면 가게로 주문 정보를 전송한다.

# Payment(결제 시스템)

* 결제가 승인되면 결과를 주문 시스템으로 알려준다.
* 결제가 취소되면 취소 사유를 주문 시스템에 알려준다.

# Store(가계 관리 시스템)

* 가게는 포인트 적립률이 있다.
* 주문 시스템으로부터 주문이 들어오면 주문을 승인 또는 취소할 수 있다.
* 주문승인 시 예상 시간을 주문 시스템에 전송한다.
* 주문취소 시 취소 사유를 주문 시스템에 전송한다.
* 가게는 메뉴를 등록, 수정, 삭제할 수 있다.
* 가게는 주문가능 시간을 기재한다.

# Point(포인트 시스템)

* 사용자의 포인트를 관리한다.
* 주문이 결제대기 상태일 때 그 포인트는 사용할 수 없다.
* 가게는 가게별로 고유의 포인트 적립률이 있다.

# User(유저 시스템)

* 유저는 아이디, 이름, 이메일, 주소를 기본으로 한다.
* 