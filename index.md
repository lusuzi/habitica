## 游戏记录

[2020年10月](202010/README.md)

[2020年11月](202011/README.md)

##  程序源码

``` python
# pseudo-code of the action in Python
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

