# scss-color-name
Name color for declare in a scss variable style

How to use? 
```
@import '[directory]/filename.scss';
```


It's a simple code which contained in a file

```scss
$abbey: #4c4f56;
$acadia: #1b1404;
$acapulco: #7cb0a1;
$aero-blue: #c9ffe5;
$affair: #714693;
$akaroa: #d4c4a8;
$alabaster: #fafafa;
$albescent-white: #f5e9d3;
```

You may have a questiion, You prefer me to use those code on my project?, The anwser is NO I prefer you copy all color and override it with you name like this 

#### Incorrect usecase
```scss
@import '[directory]/color.scss';

.button-like { 
  color: $abbey;
  background: $akaroa;
}

.main-bg { 
  background: $akaroa;
}
```

I you you as above I shown you, Please stop it. It's meaningless and heard to read.

#### Correct usecase 

```scss
// override_color.scss
@import '[directory]/color.scss';

$button_like_text: $abbey;
$button_like_bg: $akaroa;

main_bg: $akaroa;
```


```scss
@import '[directory]/override_color.scss';

.button-like { 
  color: $abbey;
  background: $akaroa;
}

.main-bg { 
  background: $akaroa;
}
```

In this case you can categorize you varible group and add meaning to those variable to color. Easy to read.
