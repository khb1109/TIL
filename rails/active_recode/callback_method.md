# 콜백 메서드

## 액티브 레코드 객체 생성하기
- before_validation
- after_validation
- before_save
- around_save
- before_create
- around_create
- after_create
- after_save
- after_commit/after_rollback

적절한 생성 제약을 돌 수 있을 것 같다.
save는 create, update를 모두 포함한다.

## 액티브 레코드 객체 업데이트하기
- before_validation
- after_validation
- before_save
- around_save
- before_update
- around_update
- after_update
- after_save
- after_commit/after_rollback

## 액티브 레코드 객체 삭제하기
- before_destroy
- around_destroy
- after_destroy
- after_commit/after_rollback

## after_initialize 와 after_find

## after_touch

---

## 콜백메서드가 생략되는 메서드들
- decrement!
- decrement_counter
- delete
- delete_all
- increment!
- increment_counter
- update_column
- pdate_columns
- update_all
- update_counters

특히 delete, delete_all, update_all은 자주사용하니 주의하자. 특히 delete 같은경우 soft delete가 생략될 수 있으니 비즈니스에 큰 문제가 생길 수 있다. 주의해서 사용하자

