# Lab 1: Git Commands

`Author:` Harrison Pinto

## Introductory Sequence

### Exercise 1

```console
git commit
git commit
```

![1.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/1.01.png)


### Exercise 2

```console
git checkout -b bugFix
```

![1.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/1.02.png)


### Exercise 3

```console
git checkout -b bugFix
git commit
git checkout main
git commit
git merge bugFix
```

![1.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/1.03.png)


### Exercise 4

```console
git checkout -b bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```

![1.04](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/1.04.png)


## Ramping Up

### Exercise 1

```console
git checkout C4
```

![2.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/2.01.png)


### Exercise 2

```console
git checkout bugFix^
```

![2.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/2.02(1).png)


### Exercise 3

```console
git branch -f main C6
git branch -f bugFix HEAD~2
git checkout C1
```

![2.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/2.03.png)


### Exercise 4

```console
git reset HEAD^
git checkout pushed 
git revert HEAD
```

![2.04](https://user-images.githubusercontent.com/30639420/165307872-802bd3f6-1cb2-4c4a-99e9-69d353aa84e4.png)


## Moving Work Around

### Exercise 1

```console
git cherry-pick C3 C4 C7
```

![2.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/2.05.png)

### Exercise 2

```console
git rebase -i overHere
```

![3.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/3.02.png)


## A Mixed Bag

### Exercise 1

```console
git checkout main
git cherry-pick C4
```

![4.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/4.01.png)

### Exercise 2

```console
git rebase -i C1
git commit --amend
git rebase -i main
git branch -f main HEAD
```

![4.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/4.02.png)

### Exercise 3

```console
git checkout main
git cherry-pick C2
git commit --amend
git cherry-pick C3
```

![4.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/4.03.png)

### Exercise 4

```console
git tag v1 side^
git tag v0 main~2
git checkout v1
```

![4.04](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/4.04.png)

### Exercise 5

```console
git commit
```

![4.05](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/4.05.png)


## Advanced Topics

### Exercise 1

```console
git rebase main bugFix
git rebase bugFix side
git rebase side another
git rebase another main
```

![5.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/5.01.png)

### Exercise 2

```console
git branch bugWork main^^2^
```

![5.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/5.02.png)

### Exercise 3

```console
git checkout one
git cherry-pick C4 C3 C2
git checkout two
git cherry-pick C5 C4 C3 C2
git branch -f three C2
```

![5.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/5.03.png)

## Push & Pull -- Git Remotes!

### Exercise 1

```console
git clone
```

![6.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.01.png)

### Exercise 2

```console
git commit
git checkout o/main
git commit
```

![6.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.02.png)

### Exercise 3

```console
git fetch
```

![6.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.03.png)

### Exercise 4

```console
git pull
```

![6.04](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.04.png)

### Exercise 5

```console
git pull
```

![6.05](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.05(1).png)

### Exercise 6

```console
git commit
git commit
git push
```

![6.06](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.06.png)

### Exercise 7

```console
git clone
git fakeTeamwork
git commit
git pull --rebase
git push
```

![6.07](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.07.png)

### Exercise 8

```console
git reset --hard o/main
git checkout -b feature C2
git push origin feature
```

![6.08](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/6.08.png)


## To Origin And Beyond -- Advanced Git Remotes!

### Exercise 1

```console
git fetch
git rebase o/main side1
git rebase side1 side2
git rebase side2 side3
git rebase side3 main
git push
```

![7.01](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.01.png)

### Exercise 2

```console
git checkout main
git pull
git merge side1
git merge side2
git merge side3
git push
```

![7.02](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.02.png)

### Exercise 3

```console
git checkout -b side o/main
git commit
git pull --rebase
git push
```

![7.03](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.03.png)

### Exercise 4

```console
git push origin main
git push origin foo
```

![7.04](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.04.png)

### Exercise 5

```console
git push origin main^:foo
git push origin foo:main
```

![7.05](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.05.png)

### Exercise 6

```console
git fetch origin main~1:foo
git fetch origin foo:main
git checkout foo
git merge main
```

![7.06](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.06.png)

### Exercise 7

```console
git push origin :foo
git fetch origin :bar
```

![7.07](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.07.png)

### Exercise 8

```console
git pull origin bar:foo
git pull origin main:side
```

![7.08](https://raw.githubusercontent.com/HASPIMA/lab01-ingesoft2/master/7.08.png)
