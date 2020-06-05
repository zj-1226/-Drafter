# -Drafter

一. 使用Drafter生成OC,swift的类图关系
  在iOS项目中自动生成类图和方法调用图 - Generate call graph in iOS project
  参考目标库： https://github.com/L-Zephyr/Drafter

类关系：
Drafter使用方法
对工程文件生成类图关系
1. 安装，会自动安装到/usr/local/bin目录中：  
	a. curl "https://raw.githubusercontent.com/L-Zephyr/Drafter/master/install.sh" | /bin/sh
	b. 也可以直接下载源码
2. cd到指定目录，然后运行：drafter -f ./AFNetworking  （-f 后面是要分析的目录）
3. 在当前目录下查看文件： ./DrafterStage/index.html

二： OmniGraffle生成UML，仅支持OC
OC UML类关系：
OmniGraffle使用方法
https://www.macxin.com/archives/10762.html
解压密码:www.macxin.com

1. 安装
2. 断网，然后使用注册机生成注册码
3. 将包含 .xcodeproj 文件的文件夹拖到OmniGraffle图标上即可

三：生成swiftUML
  swift-auto-diagram
  地址：  https://github.com/yoshimkd/swift-auto-diagram
  用法：
    How does it look like?
    They are doing an open source library (https://github.com/yoshimkd/swift-auto-diagram), which provides fast and easy generation of an html page with class diagrams of the current state of the project. How to use it? These are the three steps:

    1. Clone the git repo:

    git clone https://github.com/yoshimkd/swift-auto-diagram
    2. Run the generateClassDiagram.rb script with the path of your project as an argument:

    ruby generateEntityDiagram.rb ~/workspace/my-swift-project
    3. Open the generated html and enjoy the diagrams of your classes, structures and protocols.

四：
Clone the git repo:

git clone https://github.com/yoshimkd/swift-code-types-navigator your_local_folder

Build the tool, by running the following command in the tool’s root directory:

swift build

Run the type navigator, by typing the following command, with path/s to your Swift code:

.build/debug/SwiftDiagramGenerator . <swiftFileOrFolderPath1> <swiftFileOrFolderPath2> ...
