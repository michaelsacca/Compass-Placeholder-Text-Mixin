Compass-Placeholder-Text-Mixin
==============================

Simple Mixin For Compass Placeholder Text
		
*Steps:*

1. Add the .input-placeholder() mixin from _placeholderText.scss to your compass stylesheet (or reference it in an @import statement)
2. In your stylesheet, call the .input-placeholder() mixin anywhere you want to style your placeholder text

.inputCls {
	@include input-placeholder {
		color: #ccc;
		background: #F00;
	}
} 

Will compile to: 
				  
.inputCls.placeholder {
	color: #ccc;
	background: #F00;
}
.inputCls:-moz-placeholder {
	color: #ccc;
	background: #F00;
}
.inputCls::-webkit-input-placeholder {
	color: #ccc;
	background: #F00;
}
				  
