<h3>Run C++ in Visual studio Code with coderunner extension</h3>

Make sure you've installed code runner extension.Copy this and paste it on your settings.json file. To open settings.json in vs code command ctrl+shift+p and search settings.json
<pre>
  "code-runner.executorMap": {
        "cpp": "cd $dir && g++ $dirWithoutTrailingSlash\\$fileName -o $fileNameWithoutExt && $fileNameWithoutExt"
    
    },
</pre>

<h4>Space problem during compilation of C++ file in vscode/Space problem with cpp filename in vscode solution:</h4>

When you run a c++ file which has space in it's filename with this above code you may encouter a problem that compiler couldn't recognise the file name. The problems is with the space in filename. To solve this use the code bellow:
<pre>
 "code-runner.executorMap": {

        "cpp": "g++ $dirWithoutTrailingSlash\\\\\"$fileNameWithoutExt.cpp\" -o \"$fileNameWithoutExt.exe\" && \"$fileNameWithoutExt.exe\""
    
    },
    </pre>
