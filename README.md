# MyLisp.lsp - Simplifying AutoCAD Workflows

MyLisp.lsp is a powerful collection of tools designed to streamline your AutoCAD or BricsCAD workflows. Developed and maintained by Mohamedh Asrin, this Lisp library enhances your AutoCAD or BricsCAD experience by offering a range of convenient features.

## Prerequisites
- AutoCAD 2007 or newer // BricsCAD V15 or newer
- Windows 7 or later (tested on Windows platforms)

## Key Features
    (defun c:Lock_all ()
      (command "._layer" "lock" "*" "")
      (princ)
    )
<code>defun</code> - Calls a function</br>
<code>c:Lock_all_layers</code> -  Is the name of the function being defined.

    (command "._layer" "lock" "*" "")
The <code>command</code> function is used to send commands to AutoCAD.</br>
<code>._layer</code> is the command we are sending to AutoCAD, which allows us to interact with layers.</br>
<code>lock</code> is the subcommand that tells AutoCAD that we want to lock the layers.</br>
<code>* </code> is a parameter that accompanies the subcommand. In this case, the asterisk (*) is used to indicate that we want to apply the command to all layers in the drawing.</br>
<code>""</code> is an additional blank parameter, indicating that we don't want to specify any specific filters.</br>
The <code>princ</code> function is used to print an output to the AutoCAD command prompt to ensure that no unintended results are printed to the prompt.</br>

### To use this routine in AutoCAD:

1. Copy the code to the text area of the AutoCAD editor (either the command line or the script editing window).</br>
2. Press "Enter" to define the Lock_all_layers function.</br>
3. Type the function name (Lock_all_layers) at the command prompt and press "Enter". This will execute the function and lock all layers in the current drawing.</br>
