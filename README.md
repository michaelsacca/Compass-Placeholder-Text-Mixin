Compass-Placeholder-Text-Mixin
==============================

Simple Mixin For Compass Placeholder Text

*Syntax:*

		@mixin input-placeholder {
		  &::-webkit-input-placeholder {
		    @content;
		  }
		  &:-moz-placeholder { // Firefox 18
		    @content;
		  }
		  &::-moz-placeholder { // Firefox 19+
		    @content;
		  }
		  &:-ms-input-placeholder {
		    @content;
		  }
		}
		
*Steps:*

		1.	Add the .input-placeholder() mixin from _placeholderText.scss to your compass stylesheet (or reference it in an @import statement)
		2.	In your stylesheet, call the .input-placeholder() mixin anywhere you want to style your placeholder text

		.inputCls {
		  @include input-placeholder {
				color: #ccc;
				font-style: italic;
				font-size: 1.5em;
			} 
		} 

Will compile to: 

	  .inputCls::-webkit-input-placeholder {
			color: #ccc;
			font-style: italic;
			font-size: 1.5em;
	  }
	  .inputCls:-moz-placeholder {
			color: #ccc;
			font-style: italic;
			font-size: 1.5em;
	  }
	  .inputCls::-moz-placeholder {
			color: #ccc;
			font-style: italic;
			font-size: 1.5em;
	  }
	  .inputCls:-ms-input-placeholder {
			color: #ccc;
			font-style: italic;
			font-size: 1.5em;
	  }		
