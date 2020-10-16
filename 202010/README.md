## [HOME](../README.md)

### 10月15日

![](https://cdn.jsdelivr.net/gh/lusuzi/habitica/202010/images/15.png)

目前角色血量不够，快要死了，得赶紧升级。

暗影狐狸明天就可以驯养为坐骑。



设置全新策略，使得 [Github](https://github.com/) 各功能与 [Habitica](https://habitica.com/) 各功能环环相扣。

``` python
import Github, Habitica
from LuSuZi import break_down, simplify, just_do_it

while Alive('LuSuZi'):
    habits, tasks, todos = Habitica.output()
    for i in habits + tasks + todos:
        just_do_it(i)
        Habitica.reward()
    
    habits = Habitica.habit()
    tasks = Habitica.task()
    
    goal = Github.project()
    issues = break_down(goal)
    todos = simplify(issues)
    
    Github.time.record()
    Github.time.set(Habitica, habits, tasks, todos)
    
    day = day + 1
```

