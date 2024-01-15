# astroguard
A simple code auditing and debugger tool based on gcc for embedded C aerospace applications adhering to NASA's JPL Rule of 10.

## About

## NASA JPL Rule of 10

[Rule 1](): Avoid complex flow constructs, such as goto and recursion.

[Rule 2](): All loops must have fixed bounds. This prevents runaway code.

[Rule 3](): Avoid heap memory allocation.

[Rule 4](): Restrict functions to a single printed page.

[Rule 5](): Use a minimum of two runtime assertions per function.

[Rule 6](): Restrict the scope of data to the smallest possible.

[Rule 7](): Check the return value of all non-void functions, or cast to void to indicate the return value is useless.

[Rule 8](): Use the preprocessor sparingly.

[Rule 9](): Limit pointer use to a single dereference, and do not use function pointers.

[Rule 10](): Compile with all possible warnings active; all warnings should then be addressed before release of the software.

## Optimized Compiler [compilation.sh]:
Compilation settings should be set to the most pedantic level of operation.
Run the compilation.sh with your chosen C file to compile your selected file with those warnings.

```
chmod +x compilation.sh
compilation.sh ./snippets/Rule_1.c
```

## Testing out Snippets
```
cd snippets
gcc Rule_4.c -o Rule_4
./Rule_4
```

## References 🔬
- https://security.web.cern.ch/recommendations/en/codetools/rats.shtml
- https://code.nasa.gov/#/guide
- https://betterprogramming.pub/the-power-of-10-nasas-rules-for-coding-43ae1764f73d
- https://en.wikipedia.org/wiki/The_Power_of_10:_Rules_for_Developing_Safety-Critical_Code
- https://nasa.github.io/fprime/UsersGuide/dev/code-style.html
- https://github.com/abougouffa/awesome-coding-standards/blob/master/jpl-c-1.0.pdf

## Contributing ✨
astroguard is open to any contributions. Please fork the repository and make a pull request with the features or fixes you want to implement.

## Support 💜
If you enjoyed astroguard, please consider becoming a sponsor in order to fund my future projects.

To check out my other works, visit my [GitHub profile](github.com/ANG13T).