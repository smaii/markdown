
##TypeScript 是一种由微软开发的自由和开源的编程语言，它是JavaScript的一个超集，扩展了JavaScript的语法

#1.类型批注
	TypeScript
	通过类型批注提供静态类型以在编译时启动类型检查。这是可选的，而且可以被忽略而使用 JavaScript 常规的动态类型。
	对于基本类型的批注是number, Boolean和string。而弱或动态类型的结构则是any类型。

#2.接口
	interface Demo{
		name:String;
		age:Number;
		marriage:Boolean;
}
接口可以作为一个类型批注。