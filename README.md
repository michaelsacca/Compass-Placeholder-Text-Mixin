# Compass-Placeholder-Text-Mixin

Simple Mixin For Compass Placeholder Text
        
## Steps:

1. Add the .input-placeholder mixin from _placeholderText.scss to your stylesheet (or reference it in an @import statement)
2. In your stylesheet, call the .input-placeholder {} mixin anywhere you want to style your placeholder text

### This Scss code:

```SCSS
    input {
        @include input-placeholder {
            color: #ccc;
            background: #F00;
        }
    }
``` 

### Will compile to: 
    
```CSS
    input.placeholder {
        color: #ccc;
        background: #F00;
    }
    input:-moz-placeholder {
        color: #ccc;
        background: #F00;
    }
    input::-moz-placeholder {
        color: #ccc;
        background: #F00;
    }
    input:-ms-input-placeholder {
        color: #ccc;
        background: #F00;
    }
    input::-webkit-input-placeholder {
        color: #ccc;
        background: #F00;
    }
```
