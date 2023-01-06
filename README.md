# md

This is a repo for playing with how GitHub displays markdown formatting.

An interesting question that I saw was: 

How to wrap long lines inside of markdown ``` code ``` in Github and Gitlab issues?  
https://stackoverflow.com/questions/41238148/how-to-wrap-long-lines-inside-of-markdown-code-in-github-and-gitlab-issu

For example:  
If I want to render a code block that wraps around to next line, there currently seems to be no way of oding so using triple backtick <code>`</code> (so actually <code>```</code>)

Text entered:
````
```
this line is very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long
```
````

Below: output that is not desirable
```
this line is very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long
```

Using html tag `<code>` does allow code wrapping, but doesn't quite have the same aesthetic

<code>this line is very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long
</code>

A stackover flow user suggested adding the `<style>` tag to the file, but I can't get it to work to produce the desired result. I'm assuming I'm keeping the file type in `markdown`.

```md
<style>
code {
  white-space : pre-wrap !important;
}
</style>
```

Submit a PR or create an issue. Happy to hear your thoughts!

Related resources:  
[GitHub on Advanced Formatting](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)

<!---

Before changing this to be about `md`, this is playing with `about` / `yoyoyojoe/yoyoyojoe` as a special repository.

- 👋 Hi, I’m @yoyoyojoe
- 👀 I’m interested in ... coding!
- 🌱 I’m currently learning ... recoil
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ... https://www.linkedin.com/in/joeyma/

yoyoyojoe/yoyoyojoe is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

