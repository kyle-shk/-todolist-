## 현재 문제점

### 해당 코드에서 id는 맨처음 0으로고정시킴, 즉 컨트롤+R버튼으로 리셋을하면 다시 제 랜더링이되 id가 0으로 초기화되서 id가 중복되는 문제가 발생

- [x] id를 랜덤으로 생성하는 무언가를 새로 만들어야할듯

### 리셋전에는 crud잘되다가 리셋하고 다시 update,delete만하면 기존데이터다 삭제됨...

- [x] key에러가 있는데 이게문제인듯.. key가 명확하지않아서 다 지워지는게 아닐까?
  - key문제는 아니고 filter할때 local state에있는 data에서 filter를했는데 당연히 그렇게화면안되고 localStorage에서 저장된 데이터를 기반으로 해야 리셋이되도 데이터가 초기화되지않고 제대로 작동됨 ㅠㅠ
