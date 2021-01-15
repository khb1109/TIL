## 헷갈리는 delete_all과 delete

update와 update_all도 같은 내용이지만

delete는 모델 객체에서 사용할 수 있는 메서드다. 즉 1개의 row를 수정하는 메서드.
Model에서 바로 접근할 수 있지만, id를 명시해야한다.

delete_all은 ActiveRecord::Relation에서 접근할 수 있는 메서드다. 한번에 여러개의 로우를 설정할 수 있다.

주의할 건 update_all은 훅 메서드를 타지않는 점을 생각해야한다.