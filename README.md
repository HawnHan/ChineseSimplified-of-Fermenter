# ChineseSimplified-of-Fermenter
ChineseSimplified of Fermenter

Fermenter (发酵器)Mod兼容以下Mod列表的产物酿造/加工(请将该Mod置于以下Mod下面加载)
1.Apothecary - Composting and adds the ability to make Absinthe.
2.Multiplayer - Native support.
3.RC2 - Bottle and brewing expansion - valid fermentation recipes (needs mod researchelements).
4.RFF - Composting with spoil mash
5.SYR Blueberries. - Blueberry wine
6.VG - Garden Tools - Composting with spoil mash.
7.VG - Garden Drinks - valid fermentation recipes (needs mod research elements).
Mod允许并推荐你为自己制作清单
以下是原游戏中的将麦芽汁发酵为啤酒的例子
<Fermenter.FermentDef>
	<defName>Ferment_Beer</defName> 
	<Product>Beer</Product>
	<Resource>Wort</Resource>
	<SpoilProduct>SpoilMash</SpoilProduct>
	<FermentHours>72.0</FermentHours>
	<ResearchProject>Brewing</ResearchProject>
</Fermenter.FermentDef> 

defName: 清单唯一标志。
Product: 产物的ThingDef名称。
Resource: 所消耗的原料ThingDef名称(麦芽浆，麦芽汁，产物的前身等)。
SpoilProduct: 可选产物，如果该组材料发酵失败(变质物)。
FermentHours: 发酵所需时间。 
ResearchProject: 可选所需前置研究，研究后清单才会出现在选项中。

变质物与前置研究都是可选项，允许留空。

Mod中有一个游戏载入时运行的程序，将会检查defs中的配方成分，并给出中肯的意见。
需要注意的是你依然需要为发酵做准备工作，你需要制作物体所需的前身材料（如麦芽汁），其中包括适合无误的配方清单。

我是弟弟(译者)备注：
1.该文档源于作者的使用说明
2.Mod最小发酵周期为24小时，最长我未进行测试。（我想着也没有人会想尽可能的延长吧）
3.不允许制作产物为非食物的清单（但我未进行测试，Mod检测到会提示）
4.请不要用产物的原名作为清单组成，必须用到ThingDef名称，不要用label里面的名称（最大的区别是ThingDef不会出现空格，且多个单词组成时是驼峰写法）
5.该Mod比较贴近现实，具体表现为，当你开启显示生产过程时不允许你更换产物，生产后会进行清理过程
