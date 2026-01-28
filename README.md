# gram.py

A single file tkinter python text editor.

---

There's a simple command palette at the bottom which supports:

* Find - Find text in the editor. (ctrl-f)
* Open - Open files in the editor, accepts glob patterns. (ctrl-o)
* Tab  - Re-open tabs you have navigated away from. (ctrl-t)
* Exec - Execute arbitrary python mostly for debugging development of gram.py (ctrl-e)

Holding shift for open and tab will open a new instance.
Holding shift for find cycles backwards through finds.

---

The editor also allows for configuring the style by pressing (ctrl-m) and editing the json.


The Entry - `palette` - widget and Text - `editor` - widget `configure` funcs are passed the {"text"} dict directly.

<!-- language injection tests -->

``` cpp
#include <iostream>
int main()
{
    std::cout << "hello world" << std::endl;
    return 0;
}
```
``` python
def main():
    print("hello world")
    return 0
```
``` json
{
    "hello": "world"
}
```
``` toml
[dict.key]
hello = "world"
```