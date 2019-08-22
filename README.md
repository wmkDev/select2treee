# select2tree

### Structure
This plugin extend select2 to support treeview, allowing any level of hierarchy for ``<option>`` inside ``<select>``. 

Parent option should be referenced in children via ``data-parent`` attribute.

Sample of structure and initialization: 
```
  <select id="tree1" style="width: 550px">
    <option value="5" data-parent="">GRUPO 1</option>
    <option value="2" data-parent="5">SUBGRUPO 1.0</option>
    <option value="1" data-parent="5">SUBGRUPO 1.1</option>
    <option value="7" data-parent="1">SUBGRUPO 1.1.0</option>

    <option value="8" data-parent="1">SG 1.1.1</option>
    <option value="9" data-parent="8">SG 1.1.1.0</option>

    <option value="6" data-parent="">GRUPO 2</option>
    <option value="3" data-parent="6">SUBGRUPO 2.1</option>
    <option value="4" data-parent="6">sg 2.2</option>
  </select>
  <script>
    $("#tree1").select2tree();
  </script>
```

### Example

[Demo JSFiddler](https://jsfiddle.net/kikoDev/6vmzqbn9/)


### Screens

![Alt text](screenDemo1.png?raw=true "Demo1")
![Alt text](screenDemo2.png?raw=true "Demo2")
![Alt text](screenDemo3.png?raw=true "Demo3")

