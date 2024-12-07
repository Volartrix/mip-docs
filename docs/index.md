# Welcome 

???+ warning

    Made In Python is currently not in a usable status. Some of the features in this
    Documentation may or may not be available. Be aware!

Made In Python is a build system written in Python, where you can write Python scripts to compile or assemble all of your projects.

Example:
```py
import mip
from mip import project

proj = project.Project(name="Test", language=project.Languages.C)

proj.add_src_file("src/main.c")
proj.set_build_dir("out")
proj.set_compiler("/usr/bin/gcc")

mip.build_proj(proj=proj)
```

???+ note

    Throughout this documentation we will use the synonym "MIP" which stands
    for "Made In Python"