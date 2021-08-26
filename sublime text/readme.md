<h3>Sublime build system for CPP</h3>

To create your custom build system for c++ go to Tools>Build System>New Build System...\
<img src="assets\build.png" alt="build.png"/>\
Now copy and paste this <a href="CPP.sublime-build">CPP</a> build system on your sublime-build file and save it as CPP.sublime-build .\
Here replace your input.txt and output.txt file with path. For example if your input.txt and output.txt is in "E:/Code/" directory then the build system will be \
<code>
{
"cmd": ["g++.exe","-std=c++17", "${file}", "-o", "${file_base_name}.exe", "&&" , "${file_base_name}.exe","<E:/Code/input.txt>E:/Code/output.txt"],
"shell":true,
"working_dir":"$file_path",
"selector":"source.cpp"
}
</code>\
\
After that go to your cpp file that you want to run and select CPP as your build system and run then.\


<h3>Sublime build system for PHP</h3>

To create your custom build system for PHP go to Tools>Build System>New Build System...\
<img src="assets\build.png" alt="build.png"/>\
Now copy and paste this <a href="PHP.sublime-build">PHP</a> build system on your sublime-build file and save it as PHP.sublime-build .\
Go to your php file that you want to run and select PHP as your build system and run then.\
*Happy Coding!*