## WordPress Completions

Is a collection of WordPress completions and some snippets for Sublime Text

WordPress Version : **4.6**


### Completions

Type of completions | Nº of completions
---                 | ---
Functions           | **2666**
Filters             | **1356**
Actions             | **616**
Classes             | **327**
Methods             | **3092**
Constants           | **513**
Capabilities        | **56**


### Plugins and Themes included

Name            | Type   | Version
---             | ---    | ---
Akismet         | Plugin | **3.1.11**
Twenty Ten      | Theme  | **2.2**
Twenty Eleven   | Theme  | **2.5**
Twenty Twelve   | Theme  | **2.1**
Twenty Thirteen | Theme  | **2.0**
Twenty Fourteen | Theme  | **1.8**
Twenty Fifteen  | Theme  | **1.6**
Twenty Sixteen  | Theme  | **1.3**


### Notes

Deprecated Functions, Constants, Classes, Methods, Actions, Filters have been removed

On some cause the first "tab" deletes all parameters instead of having to tab through each one:

- First Tab --> Select all parameters
- Each Tab There after --> Selects each individual parameter or block

Actions or Filter add two version of the completion only this not is dynamic name

Example of completion file for Hooks:
```
        {
            "trigger": "add_action-init\tWP Action",
            "contents": "add_action( 'init', ${1:\\$function_to_add}${2:, ${3:10}} );"
        },
        {
            "trigger": "init\tWP Action Name",
            "contents": "init"
        },
```
This first trigger use add_action- for get all actions and continue by name of the action, returns everything you need to create.
The second trigger simply use the name and return this name.

* Use `wp-` for view some completions
* Use `add_action-` for view actions completions
* Use `add_filter-` for view filters completions
* Use functions, constants or classes names, for e.g. plugin_dir... for view completions
* Use `name_of_class-method_name` for view method completions. e.g `WP_Error-add`
  by default all Classes wrap with sublime format completions
* Use `ctrl+space` or `alt+/` in linux for call completions if tag <?php not is defined. e.g. for create plugin header in empty file.


### Other Notes

Tested on Sublime Text 3118

If use Sublime Text before 3092 is possible what some snippet not working.

If your problem with `alt+/` to show completions popup in linux, set key bindings with `ctrl+space` by example


### Install

- Find WordPress Completions in Package Control

### Issues

You found some issue, please create an issue to solve it.

### Donate

You are welcome support this project using [Paypal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=VXY7T7VKL78VA)