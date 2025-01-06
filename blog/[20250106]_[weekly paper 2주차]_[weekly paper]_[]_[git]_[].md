### Weekly Paper 2nd weeks.

#### git rebase와 git merge의 차이점을 설명하고, 각각 어떤 상황에서 사용하는 것이 적절한지 설명해주세요.

> git rebase란 : Branch의 Base를 다시 지정하는 것, commit을 재배치(rebase)하는 것을 의미합니다. 현재 branch의 base를 특정 branch로 재지정하는 것.
> git merge란 : Branch를 통합하는 것을 의미합니다.

> `merge`의 경우
> | * 034e5cc2c864ad034a0dbe5f238f1380121c0a4e (HEAD -> premium) Merge branch 'test' into premium
> | |\  
> | | * 6fa40c32218538bf8a090680e8385e3bd26b66b8 (test) Add get_Median function
> | * | 118e135a2bedd6779de268d73d644a99a04a8c32 Add get_Remainder function
> | |/  
>
> 위와 같이 merge를 이용하면, 각 commit이 통합되는 과정이 git log에서 표시된다.

> `rebase`의 경우
> | * a3258a4dd652b45039b95a3674b74af9cb10de05 (HEAD -> premium) Add get_Remainder function
> | * 6fa40c32218538bf8a090680e8385e3bd26b66b8 (test) Add get_Median function
> | * 2daf94b37d1f6e145d95ece397e3bc00d4319d58 (origin/premium) Revert "Add the info of calculator.py in README.md"
>
> 위와 같이 rebase를 이용하면, git log의 tree가 branch의 commit 단위로 나눠지지 않고, `(test) Add get_Median function`의 commit 이후에 tree가 이어집니다.


#### git fetch와 git pull의 차이점을 설명하고, 각각을 사용하는 것이 적절한 상황을 설명해주세요.

