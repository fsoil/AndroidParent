# Parent工程说明

 这是一个空的工程，保持完整的Android工程样式，为了方便编辑config文件夹下的groovy文件的时候验证语法。本项目主要的编辑区域在config文件夹下的文件，这里Android工程的各层gradle文件主要用于直接复制

> 在新建的工程根目录gradle文件依赖远程配置文件

`apply from: 'https://raw.githubusercontent.com/fsoil/AndroidParent/master/config/version/versions.gradle' `

具体参考本项目的根目录build.gradle 文件，也可以直接拷贝，替换新项目的相同文件，其他模块的gradle文件类似操作

> 添加新的依赖
  在现有的version.gradle 文件中声明的远程库不够的时候或者需要升级依赖库版本的时候可以下载此项目，进行更改然后提交新的版本，在引用的项目中同步gradle即可

> bintray文件夹下的工具用于将自己的项目提交到我们自己的maven私服进行管理，这个文件还需要在进行更改，更灵活控制
