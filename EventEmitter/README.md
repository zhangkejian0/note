# eventBus 发布/订阅事件总线

> 这里手写了一个简单eventBus,实现了事件的订阅、发布功能  
举个栗子

```
    import eventBus from '@/EventEmitter';
    
    // 定义个事件
    function eventTD(data){
        console.log('eventTD被触发',data);
    }

    // 订阅
    eventBus.on('eventBus',eventTD);

    // 发布
    eventBus.emit('eventBus', 'abc...');

    // 取消订阅
    eve.off('eventBus',eventTD);
```