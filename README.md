I want all of this to be printed as it appears after remark processes it.

Pretty much I just want non-language code fences to remain code fences.

```
This code fence has no language specified
```

```javascript
this.codeFence = 'is JavaScript'
```

I think it's a consistency issue. I'm fine if it reprints already indented code blocks as indented, but if I wrap it in a code fence it should be reprinted as a code fence.

I expect this means we'll have to store metadata on the AST for code blocks to distingish whether the source is code fenced? Maybe?

See the `output.md` file to see what the output of `remark README.md > output.md` is
