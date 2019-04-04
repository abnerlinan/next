{"title":"Addon","meta":{"title":"Addon","description":"\n","order":"6"},"codes":{"jsx":"import { Transfer } from '@alifd/next';\n\nconst dataSource = (() => {\n    const dataSource = [];\n\n    for (let i = 0; i < 10; i++) {\n        dataSource.push({\n            label: `content${i}`,\n            value: `${i}`,\n        });\n    }\n\n    return dataSource;\n})();\n\nconst obj = {\n    items: '项',\n    item: '项',\n    moveAll: '移动全部',\n    searchPlaceholder: '请输入',\n    moveToLeft: '撤销选中元素',\n    moveToRight: '提交选中元素'\n};\n\nclass Demo extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.handleChange = this.handleChange.bind(this);\n    }\n\n    handleChange(value, data, extra) {\n        console.log(value, data, extra);\n    }\n\n    render() {\n        return (\n            <Transfer id=\"a11y-transfer\" defaultValue={['2']} dataSource={dataSource} defaultLeftChecked={['1']} locale={obj} onChange={this.handleChange} titles={['Title', 'Title']} />\n        );\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n"},"body":"\n````jsx\nimport { Transfer } from '@alifd/next';\n\nconst dataSource = (() => {\n    const dataSource = [];\n\n    for (let i = 0; i < 10; i++) {\n        dataSource.push({\n            label: `content${i}`,\n            value: `${i}`,\n        });\n    }\n\n    return dataSource;\n})();\n\nconst obj = {\n    items: '项',\n    item: '项',\n    moveAll: '移动全部',\n    searchPlaceholder: '请输入',\n    moveToLeft: '撤销选中元素',\n    moveToRight: '提交选中元素'\n};\n\nclass Demo extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.handleChange = this.handleChange.bind(this);\n    }\n\n    handleChange(value, data, extra) {\n        console.log(value, data, extra);\n    }\n\n    render() {\n        return (\n            <Transfer id=\"a11y-transfer\" defaultValue={['2']} dataSource={dataSource} defaultLeftChecked={['1']} locale={obj} onChange={this.handleChange} titles={['Title', 'Title']} />\n        );\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n````","html":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nvar dataSource = function () {\n    var dataSource = [];\n\n    for (var i = 0; i < 10; i++) {\n        dataSource.push({\n            label: 'content' + i,\n            value: '' + i\n        });\n    }\n\n    return dataSource;\n}();\n\nvar obj = {\n    items: '项',\n    item: '项',\n    moveAll: '移动全部',\n    searchPlaceholder: '请输入',\n    moveToLeft: '撤销选中元素',\n    moveToRight: '提交选中元素'\n};\n\nvar Demo = function (_React$Component) {\n    _inherits(Demo, _React$Component);\n\n    function Demo(props) {\n        _classCallCheck(this, Demo);\n\n        var _this = _possibleConstructorReturn(this, (Demo.__proto__ || Object.getPrototypeOf(Demo)).call(this, props));\n\n        _this.handleChange = _this.handleChange.bind(_this);\n        return _this;\n    }\n\n    _createClass(Demo, [{\n        key: 'handleChange',\n        value: function handleChange(value, data, extra) {\n            console.log(value, data, extra);\n        }\n    }, {\n        key: 'render',\n        value: function render() {\n            return React.createElement(_next.Transfer, { id: 'a11y-transfer', defaultValue: ['2'], dataSource: dataSource, defaultLeftChecked: ['1'], locale: obj, onChange: this.handleChange, titles: ['Title', 'Title'] });\n        }\n    }]);\n\n    return Demo;\n}(React.Component);\n\nReactDOM.render(React.createElement(Demo, null), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Transfer <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> dataSource <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n    <span class=\"token keyword\">const</span> dataSource <span class=\"token operator\">=</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token keyword\">for</span> <span class=\"token punctuation\">(</span><span class=\"token keyword\">let</span> i <span class=\"token operator\">=</span> <span class=\"token number\">0</span><span class=\"token punctuation\">;</span> i <span class=\"token operator\">&lt;</span> <span class=\"token number\">10</span><span class=\"token punctuation\">;</span> i<span class=\"token operator\">++</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        dataSource<span class=\"token punctuation\">.</span><span class=\"token function\">push</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            label<span class=\"token punctuation\">:</span> <span class=\"token template-string\"><span class=\"token string\">`content</span><span class=\"token interpolation\"><span class=\"token interpolation-punctuation punctuation\">${</span>i<span class=\"token interpolation-punctuation punctuation\">}</span></span><span class=\"token string\">`</span></span><span class=\"token punctuation\">,</span>\n            value<span class=\"token punctuation\">:</span> <span class=\"token template-string\"><span class=\"token string\">`</span><span class=\"token interpolation\"><span class=\"token interpolation-punctuation punctuation\">${</span>i<span class=\"token interpolation-punctuation punctuation\">}</span></span><span class=\"token string\">`</span></span><span class=\"token punctuation\">,</span>\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token keyword\">return</span> dataSource<span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> obj <span class=\"token operator\">=</span> <span class=\"token punctuation\">{</span>\n    items<span class=\"token punctuation\">:</span> <span class=\"token string\">'项'</span><span class=\"token punctuation\">,</span>\n    item<span class=\"token punctuation\">:</span> <span class=\"token string\">'项'</span><span class=\"token punctuation\">,</span>\n    moveAll<span class=\"token punctuation\">:</span> <span class=\"token string\">'移动全部'</span><span class=\"token punctuation\">,</span>\n    searchPlaceholder<span class=\"token punctuation\">:</span> <span class=\"token string\">'请输入'</span><span class=\"token punctuation\">,</span>\n    moveToLeft<span class=\"token punctuation\">:</span> <span class=\"token string\">'撤销选中元素'</span><span class=\"token punctuation\">,</span>\n    moveToRight<span class=\"token punctuation\">:</span> <span class=\"token string\">'提交选中元素'</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">Demo</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token function\">constructor</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">props</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">super</span><span class=\"token punctuation\">(</span>props<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>handleChange <span class=\"token operator\">=</span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">handleChange</span><span class=\"token punctuation\">.</span><span class=\"token function\">bind</span><span class=\"token punctuation\">(</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">handleChange</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">return</span> <span class=\"token punctuation\">(</span>\n            <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Transfer</span></span> <span class=\"token attr-name\">id</span><span class=\"token attr-value\"><span class=\"token punctuation\">=</span><span class=\"token punctuation\">\"</span>a11y-transfer<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">defaultValue</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">[</span><span class=\"token string\">'2'</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">dataSource</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>dataSource<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">defaultLeftChecked</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">[</span><span class=\"token string\">'1'</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">locale</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>obj<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">onChange</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>handleChange<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">titles</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">[</span><span class=\"token string\">'Title'</span><span class=\"token punctuation\">,</span> <span class=\"token string\">'Title'</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span>\n        <span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Demo</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>"}