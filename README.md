# EnlightingLayout
A simple layout working as a switch on-off button - Thanks to DreaminginCodeZH for Material Progress bar


[![gif](https://github.com/ngallazzi/EnlightingLayout/blob/master/demo.gif)

# Usage

in your build.gradle (Module)
```groovy
compile 'me.ngallazzi.android.enlightinglayout:enlightinglayout:1.0.0'
```

in your build.gradle (Project)
```groovy
allprojects {
    repositories {
        jcenter()
        maven {
            url  "http://dl.bintray.com/ngallazzi/maven"
        }
    }
}
```
in your layout file (.xml)
```groovy
<com.ngallazzi.highlightingview.HighlightingView
            android:id="@+id/myEnlightingLayoutWithProgress"
            android:layout_width="120dp"
            android:layout_height="120dp"
            android:layout_margin="20dp"
            custom:idleBackgroundColor="#FFFFFF"
            custom:enlightedBackgroundColor="#FFF300"
            custom:middleText="Pale"
            custom:middleTextColor="#F6D10D"
            custom:icon="@drawable/ic_sun"
            custom:animationDurationInMillis="1500"
            custom:bottomText="sun"
            custom:bottomTextColor="#212121">
</com.ngallazzi.highlightingview.HighlightingView>
```
# Options

 - custom **idle status background color**: "custom:enlightedBackgroundColor"
 - custom **highlighted status text color**: "custom:enlightedTextColor"
 - custom **middle text*: "custom:middleText"
 - custom **middle text color*: "custom:middleTextColor"
 - custom **icon**: "custom:icon"
 - custom **animation duration**: "custom:animationDurationInMillis"
 - custom **bottom text**: "custom:bottomText"
 - custom **bottom text color**: "custom:bottomTextColor"
 
# Public Methods

 - public void setMiddleText (String text)
 - public void setBottomText(String text)
 - public void setIcon(Drawable drawable)
 - public void setHighlighted(boolean isHighlighted)
 - public boolean isHighlighted()
 - public void showProgressBar()
 - public void hideProgressBar()
 
 # License
```groovy 
Copyright 2017 Nicola Gallazzi

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
