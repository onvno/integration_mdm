# 主数据建模

主要包括实体建模，存储建模，主数据编码，主数据定义（界面建模）等方面，还可以把建模完成的实体发布到动态的主数据节点或者导出XSD文件。

## 实体建模

点击【主数据管理】→【主数据建模】→【实体建模】，进入实体建模页面，在该页面里，左边是实体的分类树，右边是对实体的分类、实体的创建，修改，删除等管理。

### 分类树管理

实体分类树是多级树结构。树根节点默认为“实体分类”。

● 新增分类

单击实体分类树的根节点“实体分类”，单击〖新增分类〗，弹出一个窗口，填写相应内容（|表示必填项）后，单击〖确认〗。

![](/articles/mdm/3-/images/image8.png)

图：新增分类

新增的主数据分类，会出现在分类树下。

● 显示分类

单击分类树下的某个主数据分类，在右边会出现该分类的信息。

![](/articles/mdm/3-/images/image9.png)

图：显示分类

● 修改分类

单击分类树下的某个主数据分类，单击〖修改〗，弹出一个窗口，填写相应内容（|表示必填项）后，单击〖确认〗。

![](/articles/mdm/3-/images/image10.png)

图：修改分类

● 删除分类。

单击分类树下的某个**主数据**分类，单击〖删除〗，弹出确认提示框，单击〖删除〗。

如果分类下存在实体的定义，则不能删除该分类。单击〖删除〗，弹出如下提示框。

![](/articles/mdm/3-/images/image11.png)

图：错误提示框

### 实体管理

系统默认，每个实体包含三个固有属性：名称（name），编码（code），描述（description）。该三个属性不能编辑，删除。

实体属性的定义项包括：

1、属性编码：唯一的英文编码标识别；

2、属性名称：中文属性名称；

3、类型：实体数据类型。包括：字符，整型，浮点型，布尔，日期，日期时间，图片，文件，下拉，大文本，时间；

4、长度：实体类型的数据宽度。当类型选择为“对象”，无长度；

5、对象类型：当类型选择为“对象”，才有效；

6、是否必输项；

7、是否唯一；

8、默认值（设置此值后，在界面会自动出现）；

9、备注。

新增实体的方式有两种：

1、新增：用户自己定义，编辑实体信息与相关属性

2、导入：用户从实体模板里选择模板后进行创建。

● 新增实体

单击分类树下的某个主数据分类，单击〖新增实体〗，从如下的下拉列表框进行选择。

![](/articles/mdm/3-/images/image12.png)

图：新增实体

1、选择“新增”方式，弹出如下窗口：

![](/articles/mdm/3-/images/image13.png)

图：新增实体

编辑实体的基本信息（|表示必填项）：实体编码，实体名称，实体分类。

单实体属性唯一校验性：勾选该实体是否单列唯一。

唯一性校验规则：用户勾选个实体属性，每一个属性的数据独立进行唯一性校验，有唯一性校验的属性列不能出现重复数据。

实体属性列表默认显示固有的三个属性：名称，编码，属性。

单击〖新增〗，会在实体属性列表的最后一行下面增加一条新行，单击每一个单元格进行编辑。

选择实体属性列表某一个属性（某一行），单击〖删除〗，直接删除该属性（该行）。

通过〖上移〗，〖下移〗可以改变属性的显示顺序。

单击〖确认〗，完成实体的新增。

2、选择“导入”方式，弹出如下窗口

![](/articles/mdm/3-/images/image14.png)

图：导入

单击“选择模板”的

![](/articles/mdm/3-/images/image15.png)

弹出如下窗口，进行实体模板的选择，单击〖确定〗。

![](/articles/mdm/3-/images/image16.png)

图：选择模板

填写“实体名称”，“实体编码”等相关信息，单击〖确定〗。

● 查看实体信息

单击某一分类下的某个实体，在页面右边会显示该实体的信息。包括：基本信息，各属性的定义。

● 修改

单击某一分类下的某个实体，单击〖修改〗，弹出实体修改窗口，修改实体基本信息或对其属性进行新增，修改，删除等编辑操作，单击〖确定〗。

● 删除

单击某一分类下的某个实体，单击〖删除〗，弹出确认提示框，单击〖删除〗。

如果该实体已经被其他系统功能模块引用，则不能删除，单击〖删除〗，弹出如下提示框

![](/articles/mdm/3-/images/image17.png)

图：错误提示框

● 生成存储&模型

生成存储&模型功能能使用户采用默认的存储定义、模型与存储的映射关系“一键式”生成，实体模型相应的存储表、模型与存储的映射关系表等。

单击某一分类下的某个实体，单击〖生成存储&模型〗，弹出实体生成存储&模型窗口，进行选项的选择。

![](/articles/mdm/3-/images/image18.png)

图：生成存储&模型提示框

● 导出Excel

单击定义树的某个分类下的某个实体，单击〖导出Excel〗，生成Excel文件（文件名为实体的编码）,包含该实体所包含的实体属性，保存到浏览器所在的机器。

● 复制实体

为了帮助用户快速创建实体模型，单击某一分类下的某个实体，单击〖复制〗,会弹出“复制实体”窗口，该实体的建模相关内容随即带出，用户可以直接修改，确认后，快速得到一个新实体模型。

## 存储表定义

点击【主数据管理】→【主数据建模】→【存储表定义】，进入存储表定义页面，在该页面里，上边是存储表列表，下边是每个存储表的字段定义列表。

系统默认，每个存储表包含三个固有字段：名称（name），编码（code），描述（description）。不能编辑，删除。

● 新增

单击〖新增〗，会弹出如下窗口。

![](/articles/mdm/3-/images/image19.png)

图：新增存储表

编辑存储表定义的基本信息（*表示必填项）：名称，表名称，备注。

单击〖新增〗，会在字段列表的最后一行下面增加一条新行，单击每一个单元格进行编辑。

其中，编辑列以及约束如下：

→ 名称： 显示中文意思的数据库表结构中字段代表的真实意义；

→ 字段名称： 数据库表的列字段名称，使用英文及缩写符合数据库列名规范；

→ 字段类型： 可选择如下字段类型:字符型、可变字符型、16位整型、32位整型、精确数值型、近似数值型、日期型、日期时间型、时间戳、布尔型、ID/PK、二进制；

→ 字段长度：字段允许的最大宽度。

选择字段列表的某一行，单击〖删除〗，直接删除该字段定义（该行）。

通过〖上移〗，〖下移〗可以改变字段的显示顺序。

单击〖确认〗，完成存储表的新增。

● 查看信息 

单击存储表列表里某一个存储表行，在下边会联动显示该存储表的相关信息，包括：名称，字段名称，字段类型，字段长度，备注。

● 修改

单击存储表列表里某一个存储表行，单击〖修改〗,弹出存储表修改窗口，修改存储表的基本信息或对其字段进行新增，修改，删除，上移，下移等编辑操作，单击〖确定〗。

注：在字段列表会显示系统默认的三个固有字段：名称（name），编码（code），描述（description）。

● 删除 

单击存储表列表里某一个存储表行，单击〖删除〗，弹出确认提示框，单击〖删除〗。

● 读取表

用户可以直接从系统数据库选择某个表作为存储表，单击〖读取表〗，弹出如下窗口。

![](/articles/mdm/3-/images/image20.png)

图：读取表

单击某一行作为存储表，单击〖确认〗。

用户输入相关信息，单击 

![](/articles/mdm/3-/images/image21.png)

可以对数据库表进行模糊定位。

## 存储模型

单击【主数据管理】→【主数据建模】→【存储模型】，进入存储模型页面，在该页面里，左边是实体分类树，以便主数据实体的选择，右边是实体与存储表的映射关系的管理。

实体类型与存储表定义类型的映射关系如下：

<table>

 <tr>

 <td>实体属性类型</td>

 <td>存储表定义类型</td>

 </tr>

 <tr>

 <td>字符、大文本、 、图片、对象、文件、下拉</td>

 <td>VARCHAR</td>

 </tr>

 <tr>

 <td>布尔</td>

 <td>BOOLEAN</td>

 </tr>

 <tr>

 <td>整型</td>

 <td>INT</td>

 </tr>

 <tr>

 <td>浮点</td>

 <td>FLOAT</td>

 </tr>

 <tr>

 <td>日期</td>

 <td>DATE</td>

 </tr>

 <tr>

 <td>日期时间</td>

 <td>DATETIME</td>

 </tr>

</table>


存储模型主要功能是维护实体与存储表以及它们属性之间的映射关系。

●

该“建立映射关系”操作只是业务逻辑上建立了映射关系，物理上建立映射关系，需要进行“同步数据库表”的操作。

单击主数据分类树的某个分类下的某个实体，单击〖修改〗，弹出“修改存储模型”窗口。窗口下方有主数据实体子表与新增存储表字段的映射关系对应列表，因为还没选择存储表，故“新增存储表字段”列为空。

![](/articles/mdm/3-/images/image22.png)

图：建立映射关系

单击“新增存储表”右侧的 

![](/articles/mdm/3-/images/image15.png)

弹出如下的类似端口，进行存储表的选择。单击某一行（某个存储表），单击〖确定〗。

![](/articles/mdm/3-/images/image23.png)

图：选择存储表

在映射关系对应表，依次单击每个映射关系行，单击每行右侧的

![](/articles/mdm/3-/images/image15.png)

弹出如下类似窗口，对该行的实体属性对应在存储表的字段进行选择，选择完毕后，单击〖确定〗。

![](/articles/mdm/3-/images/image24.png)

图：选择对应的字段

返回“修改存储模型”窗口，依次对实体属性在存储表的字段的映射关系进行配置，配置完毕后，单击〖确定〗。

●

单击分类树的某个分类下的某个实体，单击〖删除〗，消除此实体的全部属性在存储表的全部映射关系。“新增存储表字段”列则改变为空。

● 同步数据库表

单击分类树的某个分类下的某个实体，单击〖同步数据库表〗，在物理上，也即数据库里，建立了实体与存储表以及实体属性与存储表字段的映射关系。

## 主数据编码

单击【主数据管理】→【主数据建模】→【主数据编码】，进入主数据编码页面，在该页面里，左边是实体的分类树，以便实体的选择，右边是该主数据编码的管理。

主数据编码由以下四种元素类型组成：

1) 常量：即固定值，表示固定字符串和分隔符，长度取字符串长度；

2) 实体属性：取实体的某一属性值作为编码的一部分；

3) 日期：主数据产生的日期；

4) 流水号：主数据的顺序号。

在主数据编码规则定义中，四个元素组合使用。

● 查看编码规则

单击实体分类树的某个分类下的某个实体，在页面右边会显示该实体的编码信息，包括：规则编码，规则名称，编码长度，编码展示效果，以及编码规则的各元素的组成等。如果该实体未定义编码规则，则各显示项无内容。

● 修改

单击实体分类树的某个分类下的某个实体，单击〖修改〗，弹出如下窗口，它包括：编码的基本信息以及编码规则列表。

在编码基本信息编辑中。

1) 含|的是必填项；

2) 时间格式：在编码规则中日期显示的格式。比如当前日期为20141203，不同格式显示如下：

<table>

 <tr>

 <td>时间格式</td>

 <td>示例</td>

 </tr>

 <tr>

 <td>yy</td>

 <td>14</td>

 </tr>

 <tr>

 <td>yyyy</td>

 <td>204</td>

 </tr>

 <tr>

 <td>yyMM</td>

 <td>1412</td>

 </tr>

 <tr>

 <td>yyyyMM</td>

 <td>201412</td>

 </tr>

 <tr>

 <td>yyMMdd</td>

 <td>141203</td>

 </tr>

 <tr>

 <td>yyyyMMdd</td>

 <td>20141203</td>

 </tr>

</table>

表：时间格式

3) 编码长度：主数据编码的总长度，它等于各元素的各长度的总和，它随着用户编辑编码元素的长度而动态变化；要求总长度不可超过32，流水号长度不可超过10位。

4) 显示效果：最终的主数据编码样式。它随着用户编辑编码元素而动态变化。

在编码规则列表的编辑中，

1) 单击〖新增〗，会在列表最后一行后增加一行；

2) 单击〖删除〗，删除列表中的选定行；

3) 单击〖上移〗，列表中的选定行向上移动一行；

4) 单击〖下移〗，列表中的选定行向下移动一行；

5) 单击〖置项〗，列表中的选定行移动到第一行；

6) 单击〖置底〗，列表中的选定行移动到最后一行；

编码元素编辑中，可以对编码的四种元素的个数，位置进行随意组合。

![](/articles/mdm/3-/images/image25.png)

图：新增编码规则

对于编码规则的实体类型的元素值，单击

![](/articles/mdm/3-/images/image15.png)

弹出窗口进行定位选择。

● 删除

单击主数据分类树的某个分类下的某个实体，单击〖删除〗，则该实体的编码规则被清除。如果该实体未定义编码规则，则〖删除〗不可用。

● 扩展接口

为了满足客户定制化的需求，用户可以实现编码规则扩展接口定义，注册到主数据管理，这样生成编码规则时调用

选择“编码规则”窗口的扩展接口的“扩展接口”的单选按钮。

## 主数据定义

单击【主数据管理】→【主数据建模】→【主数据定义】，进入主数据定义页面，在该页面里，左边是主数据的定义分类树，右边是分类下主数据实体定义的管理。

主数据定义是主数据界面模型设计。

→ 支持单表，主子表（可支持多子表）、树表、树卡、表树；

→ 支持生成基础菜单，即生成的页面可以进行新增，修改，删除等操作；

→ 〖设置主表字段〗，指设置单表或主子表的主表的显示字段的可见性、必输项、快速查询条件定义、各种参照编辑；

→ 〖设置子表字段〗，指设置主子表的子表的显示字段的可见性、必输项、快速查询条件定义、各种参照编辑，子表字段支持多子表；

→ 〖自定义按钮〗，指发布的主数据页面上可添加按钮，支持用户自定义发布后主数据的相关按钮与操作，结果在发布的主数据页面上查看新增自定义按钮；

![](/articles/mdm/3-/images/image26.png)

图：自定义按钮

→ 〖导出Excel〗，指把主数据的各属性导出为Excel格式文件；

→ 不同的实体属性的定义会得到不同的页面控件。例如：

<table>

 <tr>

 <td>实体属性类型</td>

 <td>页面控件</td>

 </tr>

 <tr>

 <td>字符</td>

 <td>文本框（text）</td>

 </tr>

 <tr>

 <td>数字，浮点</td>

 <td>文本框（text）</td>

 </tr>

 <tr>

 <td>日期</td>

 <td>日期选择器</td>

 </tr>

 <tr>

 <td>对象</td>

 <td>对象参照 </td>

 </tr>

 <tr>

 <td>布尔</td>

 <td>单选按钮（radiobutton）</td>

 </tr>

 <tr>

 <td>大文本</td>

 <td>多行的文本框（textarea）</td>

 </tr>

 <tr>

 <td>下拉</td>

 <td>下拉列表框</td>

 </tr>

 <tr>

 <td>时间</td>

 <td>时间控件</td>

 </tr>

</table>

表：实体属性与页面控件的对应

→ 可以查看最终页面的生成效果。页面右边的

![](/articles/mdm/3-/images/image29.png)

虚线框范围是页面效果；

→ 最终的生成页面默认包含常用查询与高级查询，常用查询的属性可自定义；

→ 可以查看“卡片界面预览”的在主数据创建、修改时的展示结果；

→ 已经发布的主数据节点不能再进行主数据定义。

### 分类树管理

主数据定义分类树支持多层树结构。树根节点默认为“主数据”。

●

单击定义分类树的根节点“主数据”，单击〖新增分类〗，弹出一个窗口，填写相应内容（|表示必填项）后，单击〖确认〗。

![](/articles/mdm/3-/images/image30.png)

图：新增分类

新增的分类，会出现在分类树下。

●

单击分类树下的某个定义分类，在右边会出现该定义分类的信息。

● 修改

单击定义分类树下的某个定义分类，单击〖修改〗，弹出一个窗口，填写相应内容（|表示必填项）后，单击〖确认〗。

![](/articles/mdm/3-/images/image31.png)

图：修改分类

● 删除

单击分类树下的某个定义分类，单击〖删除〗，弹出确认提示框，单击〖删除〗。

如果分类下存在实体的定义，则不能删除该分类。单击〖删除〗，弹出如下提示框。

![](/articles/mdm/3-/images/image32.png)

图：错误提示框

### 主数据定义

● 新增主数据

单击定义树的某个分类，单击〖新增主数据〗，弹出新窗口，输入如下内容，单击〖确定〗

→ 基本信息。编码、名称、排序字段、所属分类（含|的是必填项）、扩展条件。

→ 界面信息。简单UI模型（单表、主子表）定义；复杂UI模型（树卡、树表、表树）的定义；是否生成基础菜单、

![](/articles/mdm/3-/images/image33.png)

图：新增定义

其中界面信息的选择有：

1)主子表（即界面上边是主表，下边是主表相关的子表）；

![](/articles/mdm/3-/images/image34.png)

2)树卡（即界面左边是树状结构，右边是卡片形式）；

![](/articles/mdm/3-/images/image35.png)

3)树表（即界面左边是树状结构，右边是表格形式）；

![](/articles/mdm/3-/images/image36.png)

4)表树（即在表格里有树状结构数据）；

![](/articles/mdm/3-/images/image37.png)

5）选择“流程特性”，则表明该主数据申请、修改等要走相关“流程”。

新增完毕，可以在〖设置主表字段〗或〖设置子表字段〗、〖自定义按钮〗对界面模型进一步编辑。

单击〖设置表头字段〗或〖设置子表字段〗、〖自定义按钮〗弹出的窗口如下：

![](/articles/mdm/3-/images/image38.png)

图：设置表头字段

其中：

**“编辑字段”页签**，可以设置各实体属性在界面：

1）是否可见；

2）是否是必输项，如果是，则在界面上字段后面有|，表明必填，若不填会有相应提示；

3）是否加入到快速查询条件；

4）增加字段“校验规则”，点击打开校验规则的维护选择界面，可以自定义校验规则，填入正则表达式或自定义java类来校验主数据的某个字段的值是否合法。主数据装载的时候会进行校验。

![](/articles/mdm/3-/images/image39.png)

图：校验规则

“编辑参照”页签，可以设置各种类型的参照，例如：多选参照、树表参照等。

其中，对象和下拉类型不仅能参照其他主数据也能参照自身。

● 更新定义

单击定义树的某个分类下的某个实体，单击〖更新〗，弹出窗口，修改内容（编码项不能修改），单击〖确定〗。

更新完毕，可以在〖设置表头字段〗或〖设置表体字段〗对界面模型进一步编辑，也可以查看〖卡片界面显示〗。

● 删除

单击定义树的某个分类下的某个实体，单击〖删除〗,会弹出删除确认框，单击〖是〗。如果主数据定义已经发布，则不能删除，会弹出如下提示框。

![](/articles/mdm/3-/images/image40.png)

图：错误信息框

● 导出定义

单击定义树的某个分类下的某个实体，单击〖导出〗，生成XSD文件（文件名为主数据定义的编码），保存到浏览器所在的机器。

● 导出Excel

单击定义树的某个分类下的某个实体，单击〖导出Excel〗，生成Excel文件（文件名为主数据定义的编码）,包含该实体所包含的实体属性，保存到浏览器所在的机器。导出EXCEL支持多子表。

## 实体模板

单击【主数据管理】→【主数据建模】→【实体模板】，进入实体模板页面，在该页面里，左边是主数据的模板分类树，右边是分类下主数据实体模板的管理。

### 分类树管理

模板分类树支持多层树结构。树根节点默认为“模板分类”。

● 新增分类

单击定义分类树的根节点“模板分类”，单击〖新增分类〗，弹出一个窗口，填写相应内容，其中：

→ |表示必填项；

→ 内置：选择此选项，则表明该模板是系统内置模板。

单击〖确认〗，新增的模板分类，会出现在分类树下。

![](/articles/mdm/3-/images/image41.png)

图：新增分类

●

单击分类树下的某个模板分类，在右边会出现该模板分类的相关信息。

● 修改

单击定义分类树下的某个模板分类，单击〖修改〗，弹出一个窗口，填写相应内容（*表示必填项）后，单击〖确认〗。

![](/articles/mdm/3-/images/image42.png)

图：修改分类

● 删除

单击分类树下的某个模板分类，单击〖删除〗，弹出确认提示框，单击〖删除〗。

如果分类下存在模板，则不能删除该分类。单击〖删除〗，弹出如下提示框。

![](/articles/mdm/3-/images/image43.png)

图：错误提示框

### 模板管理

● 新增模板

单击分类树下的某个模板分类，单击〖新增模板〗，弹出“新增模板”窗口，输入或操作相关内容：

→ 基本信息：包括：模板名称，模板编码，备注。模板来源不需要用户输入，只是显示标示；

→ 模板属性列表：包含〖新增〗，〖删除〗，〖上移〗，〖下移〗以及在列表中各模板属性的编辑，其操作方式跟【实体建模】的实体属性列表的操作类似。

![](/articles/mdm/3-/images/image44.png)

图：新增模板

● 导入模板

单击分类树下的某个模板分类，单击〖导入模板〗，会出现下拉框，

→ 选择“实体”，弹出如下窗口，选择相关实体对象，输入相关内容，单击〖确定〗。

![](/articles/mdm/3-/images/image45.png)

图：导入模板

→ 选择“XSD”，弹出“导入XSD”窗口，单击〖选择文件〗，弹出向导窗口，在浏览器所在机器定位文件。

● 查看模板

单击分类树下的某个模板分类下的某个模板，页面右边显示该模板的相关信息，包括基本信息以及模板属性列表。

● 删除

单击分类树下的某个模板分类下的某个模板，单击〖删除〗,会弹出删除确认框，单击〖是〗。如果该模板被系统其他模板引用，则不能删除，弹出相应提示框。

● 导出模板

单击分类树下的某个模板分类下的某个模板，单击〖导出〗，生成XSD文件（文件名为模板编码），保存到浏览器所在的机器。