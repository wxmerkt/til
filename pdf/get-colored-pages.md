```
function get_colored_pages() {
  gs -o - -sDEVICE=inkcov $1 |tail -n +4 |sed '/^Page*/N;s/\n//'|sed -E '/Page [0-9]+ 0.00000  0.00000  0.00000  / d'
 }
 ```
