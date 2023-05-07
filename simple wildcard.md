simple wildcard
========================
simple wildcard for ComfyUI
* web: https://civitai.com/models/21611/
* repo: https://github.com/lilly1987/ComfyUI_node_Lilly

```

ex : {3$$a1|{b2|c3|}|d4|{-$$|f|g}|{-2$$h||i}|{1-$$j|k|}}/{$$l|m|}/{0$$n|}

{1|2|3} -> 1 or 2 or 3

{2$$a|b|c} -> a,b or b,c or c,a or bb or ....

{9$$a|b|c} -> {3$$a|b|c} auto fix max count

{1-2$$a|b|c} -> 1~2 random choise

{-2$$a|b|c} -> {0-2$$a|b|c} 0-2

{1-$$a|b|c} -> {0-3$$a|b|c} 1-max

{-$$a|b|c} -> {0-3$$a|b|c} 0-max

{9$$ {and|or} $$a|b|c} -> a or b or c / c and b and a

```

install : ComfyUI\custom_nodes\ComfyUI_node_Lilly

txt folder :

ComfyUI\wildcards

or edit line

card_path=os.path.dirname(__file__)+"\\..\\wildcards\\**\\*.txt"





https://civitai.com/user/lilly1987