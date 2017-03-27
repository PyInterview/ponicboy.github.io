---
layout: page-fullwidth
title:  "The Full-Width Page Template"
subheadline:  "Multi-Device Layouts"
breadcrumb: true
teaser: "The full-width page format gives you all the space you need to show your content using the grid."
categories:
    - review
---
---


OK lets learn stacks!



<style type="text/css" media="screen">
    #editor {
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
    }
    #editorContainer {
        width: 600px;
        height: 500px;
        position: relative;

    }
</style>

<div id="editorContainer">
<div id="editor">function foo(items) {
# Problem:
# Given a string of opening and closing parentheses, check whether it’s balanced.

def isBalanced(expr):
    if len(expr)%2!=0:
        return False
    opening=set('([{')
    match=set([ ('(',')'), ('[',']'), ('{','}') ])
    stack=[]
    for char in expr:
        if char in opening:
            stack.append(char)
        else:
            if len(stack)==0:
                return False
            lastOpen=stack.pop()
            if (lastOpen, char) not in match:
                return False
    return len(stack)==0

# Test Cases:
print isBalanced('()()(()))')
}
</div>
</div>



<script src="https://cdn.jsdelivr.net/ace/1.2.6/noconflict/ace.js" type="text/javascript" charset="utf-8"></script>

<script>
    var editor = ace.edit("editor");
    editor.getSession().setUseWorker(false);
    editor.setTheme("ace/theme/xcode");
    editor.getSession().setMode("ace/mode/javascript");
    editor.getSession().setMode("ace/mode/python");
    document.getElementById('editor').style.fontSize='12px';

    editor.getSession().setUseWrapMode(true);
    editor1.setAutoScrollEditorIntoView(true);


</script>


### Step 3

Add the include whereever you want in your content with `{% raw %}{% include gallery %}{% endraw %}`.

{% include alert info='Have a look at this example-entry. And have a look into the images-folder. :)' %}











## Other Post Formats
{: .t60 }
{% include list-posts tag='post format' %}



 [1]: http://foundation.zurb.com/docs/components/clearing.html
 [2]: http://foundation.zurb.com/docs/components/block_grid.html
 [3]: {{ site.url }}{{ site.baseurl }}/design/page/
 [4]: {{ site.url }}{{ site.baseurl }}/design/page-fullwidth/
