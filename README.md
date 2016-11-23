<h2>Hello-React</h2>
React 学习总结<br/>
GitHub上开源项目：https://github.com/facebook/react
<hr/>
<h3>1、<b>什么是<a href="http://www.ruanyifeng.com/blog/2015/03/react.html">React</a>?</b></h3>
React is a JavaScript library for building user interfaces.<br/>
<p>React是一个JavaScript库，用来构建用户界面，为数据渲染视图</p>
<ul>
特点：
<li>声明式设计</li>
<li>高效：React虚拟DOM，最大限度的减少与DOM的交互</li>
<li>灵活：方便与其它库搭配起来</li>
<li>组件：构建组件</li>
<li>JSX：js语法的扩展，允许在js中写HTML</li>
<li>状态：内容与状态对应起来</li>
</ul>
<p>copy以下阮一峰大神的React入门实例中的原话来介绍以下React:</p>
<p>&nbsp;&nbsp;<b>React 起源于 Facebook的内部项目，由于不满意市面上的<a href="http://www.ruanyifeng.com/blog/2015/02/mvcmvp_mvvm.html">JavaScript MVC 框架</a>,决定自己开发一套来架设Instaram网站，然后咋2013年5月开源了。</b></p>
由于React的设计思想及其独特，属于革命性创新，性能出众，代码逻辑却非常简单，可能认为将是Web开发的主流工具。
<p>试想一下如果用Web App的方式去写Native App。那将会颠覆整个互联网行业</p>
<h3>2、核心思想</h3>
分装组件、各个组件维护自己的状态和UI，当状态改变，自动更新组件，适合功能复杂的应用：组件驱动的开发。
<h3>3、核心概念</h3>
<ul>
	<li>组件</li>
	<li>JSX(用jsx语法取代HTML，在js中描述UI)jsx浏览器不识别，需要转换为js代码(babel将jsx转换为js)</li>
	<li>
	<p>虚拟DOM</p>
	<p>diff算法：当更新组件的时候，会通过diff算法寻找到需要更新的DOM 节点，虚拟DOM是存在内存的js数据结构 性能比原生DOM好</p>
	</li>
	<li>数据流：单向数据流(状态与内容)</li>
</ul>
<h3>4、搭建React开发环境</h3>
引入三个js文件
<ul>
	<li>react.js(React的核心库)</li>
	<li>react-dom.js(提供与DOM相关的功能)</li>
	<li>browser.js(将JSX语法转换为JavaScript语法)</li>
	<li><script type="text/babel"></script></li>
</ul>
<h3>5、JSX</h3>
基本语法：
<p>遇到HTML标签,使用HTML来解析</p>
<p>遇到代码块({}),使用js解析</p>
<h3>6、组件</h3>
<h4>6.1、创建组件</h4>
var HelloMsg = React.createClass(); 
<h4>6.2、使用组件</h4>
<HelloMsg/>
注意事项：<br/>
<p>1、组件的命名：首字母必须大写。</p>
<p>2、在渲染组件，返回要求只有一个标签，但是这个标签可以包含多个子元素。</p>
<h4>6.3、复合组件</h4>
<p>将其他的组件整合在一起 创建一个新的组件</p>
<p>例子：使用复合组件实现登录窗口</p>
<h3>7、ref</h3>
如果从组件获得真实的DOM的节点，ref属性<br/>
//通过指定ref='ref名字'-->this.refs.ref名字<br/>
<div style="background: #eee;">
	<input type="text" ref="inputTxt"/>
	function(){
	this.refs.inputTxt-->拿到真实的DOM节点
}
</div>
<h3>demo将会放在code和issues里面</h3>
