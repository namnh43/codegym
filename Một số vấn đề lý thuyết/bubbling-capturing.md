#### Tham khảo: https://javascript.info/bubbling-and-capturing
## Một số  nội dung cần nhớ
### Bubbling
Khi 1 sự kiện (event) xảy ra trên 1 element, đầu tiên nó sẽ thực hiện handler trên element đó, sau đó sẽ truyền event đó lên phần tử cha (nếu cha định nghĩa 1 hàm hander cho event thì sẽ thực thi hàm handler đó)
#### event.target
* 1 handler trên element cha luôn có thể lấy được chi tiết về nơi mà event đó xảy ra thông qua event.target
* The most deeply nested element that caused the event is called a target element, accessible as event.target
* Note the differences from this (=event.currentTarget):

* event.target – is the “target” element that initiated the event, it doesn’t change through the bubbling process.
* this – is the “current” element, the one that has a currently running handler on it.
#### Stopping bubbling
The method for it is event.stopPropagation().  
_*Don’t stop bubbling without a need!_
### Capturing
The standard DOM Events describes 3 phases of event propagation:

* Capturing phase – the event goes down to the element
* Target phase – the event reached the target element.
* Bubbling phase – the event bubbles up from the element.