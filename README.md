# stack-multi-exes-example

Please note I do not understand this problem well. Below is a vague best guess of what is happening. Issues/PRs welcome to provide proper explanations.

1. The module containing the function `main` must be called `Main`
2. You cannot have two modules named `Main` in the same directory
3. However, it is ok to call the file containing the module `Main` something else (`Exe2.hs` in our example)

If everything is working, you should be able to clone this repo and run

```bash
> stack build
[build output]
> stack exec exe1
someFunc
> stack exec foo
"foo"
```

