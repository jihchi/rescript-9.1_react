# ReScript 9.1 does not support rescript/react 0.10.1

* [[ANN] rescript 9.1 for beta testing (windows testing welcome!)](https://forum.rescript-lang.org/t/ann-rescript-9-1-for-beta-testing-windows-testing-welcome/1427)
* [rescript-react](https://github.com/rescript-lang/rescript-react)

You'd get an error when you execute the command `npm run build`:

```sh
> rescript build

rescript: [1/1] src/demo.cmj
FAILED: src/demo.cmj

  We've found a bug for you!
  /Users/<name>/<repo>/src/demo.res:10:4-9

   8 │   let msg = "Click me " ++ times
   9 │
  10 │   <button> {msg->React.string} </button>
  11 │ }
  12 │

  The module or file ReactDOMRe can't be found.
  - If it's a third-party dependency:
    - Did you list it in bsconfig.json?
    - Did you run `bsb` instead of `bsb -make-world`
      (latter builds third-parties)?
  - Did you include the file's directory in bsconfig.json?

FAILED: cannot make progress due to previous errors.
```
