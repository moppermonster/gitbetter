# gitbetter

This repo serves as a starting point for playing/practicing usage of the `git` program.

This exercise assumes users already know about and can work with:
- `git clone`
- `git add`
- `git commit`
- `git push`
- `git pull`
- `git branch`
- `git checkout`

Follow the instructions in the readme to learn about merge conflicts and rebasing.

## Usage instructions
This excersise is most efficient with at least one other person.

One person will be the *maintainer* and at least one other person will be the *contributor*.

> It is possible to have several *contributors* but there should be only one *maintainer*.

### Step 1: Forking
1. The first step is quite simple: the *maintainer* makes a fork of this repository.

2. The second step involves *contributors* forking the *maintainer*'s repo.

### Step 2: Add something
1. The *contributors* will make a change to their repo.

First, create a new feature branch called `cya`.

2. Add a new feature to the `program.py` script.

Add the following:

```python3
def bye():
    '''Bye world'''
    print('bye world')
```

3. Add and commit (`-m "add bye"`) your change. Don't push!

4. Add another thing:

```python3
def toodles():
    '''Toodles world'''
    print('toodles world')
```

5. Add and commit (`-m "add toodles"`) your change. Don't push!

6. All *contributors* should now have a repo containing a feature branch `cya` containing 2 new commits.

### Step 3: Preparing for merge
1. The *maintainer* asks all *contributors* to use `git rebase` to squash the commits in the `cya` feature branch into one.

### Step 4: Merge
1. Finally, the *contributors* will ask the *maintainer* to merge their code.

### Step 5: Start a conflict
1. If there is only one *contributor*, the *maintainer* can play the role of *contributor* from here on.

2. Try and create a problem:

All *contributors* creates a new feature branch (pick a logical name reflecting the name of the function you will add to `program.py`) containing a new function as done during step 2. Yes; you can come up with a name this time.

> If you have more than one contributor, make sure that everyone is adding a feature with a different name.

3. Add, commit and push, then request to merge your changes into the *maintainer*'s fork.

4. What do you expect to happen?

5. Fix any merge conflicts.

### Step 6: Uh oh
1. All *contributors* will change the original `hello()` function to print something else.

2. Add, commit and push, then request to merge your changes into the *maintainers*'s fork.

4. What do you expect to happen?

5. Fix any merge conflicts.

## Tips:

- Don't panic
- Work together, not against eachother

Good luck and have fun!
