# Morph Bottom Navigation 


This library represents a Bottom Navigation with an awesome morph effect on top of the selected item.

![ezgif com-crop](https://user-images.githubusercontent.com/15737675/41735760-d633e706-758a-11e8-9f30-3f07c8ed4371.gif)

Don't forget to star the project if you like it! 
![star](https://user-images.githubusercontent.com/15737675/39397370-85f5b294-4afe-11e8-9c02-0dfdf014136a.png)
 == ![heart](https://user-images.githubusercontent.com/15737675/39397367-6e312c2e-4afe-11e8-9fbf-32001b0165a1.png)
 
 And feel free to submit issues and enhancement requests !
 
 ![ezgif com-video-to-gif](https://user-images.githubusercontent.com/15737675/41736506-026b6fd6-758d-11e8-9be6-7bc217aaa1e8.gif)
![ezgif com-video-to-gif 1](https://user-images.githubusercontent.com/15737675/41736508-03b14cf8-758d-11e8-8bef-3909528f405d.gif)
![ezgif com-video-to-gif 2](https://user-images.githubusercontent.com/15737675/41736510-04dc9ce0-758d-11e8-9951-11d924ebc6b0.gif)


## How to
#### Gradle
```Gradle
dependencies {
    implementation 'com.github.TalebRafiepour:BottomNavigationView:0.0.2'
}


allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
#### Usage
`MorphBottomNavigationView` extends the `BottomNavigationView` from the official [Google Material Component repository](https://github.com/material-components/material-components-android), so you can use it as described on the [Android Developers documentation](https://developer.android.com/reference/com/google/android/material/bottomnavigation/BottomNavigationView)

#### In your XML layout
```Xml
<com.tbuonomo.morphbottomnavigation.MorphBottomNavigationView
    android:id="@+id/bottomNavigationView"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    app:layout_constraintBottom_toBottomOf="parent"
    app:menu="@menu/menu_bottom_navigation"
    app:backgroundTint="@color/colorPrimary"
    app:morphCornerRadius="128dp"
    app:morphItemRadius="64dp"
    app:morphVerticalOffset="8dp"
    app:fontAssetSrc="fonts/IranSans.ttf"
    style="@style/BottomNavigationView"
    />
```


### In your styles
```
<style name="BottomNavigationView" parent="Widget.MaterialComponents.BottomNavigationView">
        <item name="itemBackground">@drawable/background_bottom_nav_item</item>
        <item name="itemIconTint">@drawable/color_bottom_nav_item</item>
        <item name="itemTextColor">@drawable/color_bottom_nav_item</item>
        <item name="itemTextAppearanceActive">@style/TextAppearance.BottomNavigation.Overline</item>
        <item name="itemTextAppearanceInactive">@style/TextAppearance.BottomNavigation.Overline</item>
        <item name="textAllCaps">true</item>
        <item name="paddingStart">32dp</item>
        <item name="paddingEnd">32dp</item>
    </style>

    <style name="TextAppearance.BottomNavigation.Overline" parent="TextAppearance.MaterialComponents.Overline">
        <item name="android:textSize">8sp</item>
    </style>
```

### Or If You Want To Responsive Dimen Then You Can Use Below Dimen To Override

```
<dimen name="design_bottom_navigation_active_item_max_width">168dp</dimen>
<dimen name="design_bottom_navigation_active_item_min_width">96dp</dimen>
<dimen name="design_bottom_navigation_active_text_size">14sp</dimen>
<dimen name="design_bottom_navigation_elevation">8dp</dimen>
<dimen name="design_bottom_navigation_height">56dp</dimen>
<dimen name="design_bottom_navigation_icon_size">24dp</dimen>
<dimen name="design_bottom_navigation_item_max_width">96dp</dimen>
<dimen name="design_bottom_navigation_item_min_width">56dp</dimen>
<dimen name="design_bottom_navigation_margin">8dp</dimen>
<dimen name="design_bottom_navigation_shadow_height">1dp</dimen>
<dimen name="design_bottom_navigation_text_size">12sp</dimen>
```


#### Custom Attributes
| Attribute | Description |
| --- | --- |
| `backgroundTint` | Color of the bottom navigation background |
| `morphCornerRadius` | Radius in dp of the morph corners (by default 128dp) |
| `morphItemRadius` | Radius in dp of the morph item circle shape (by default 64dp) |
| `morphVerticalOffset` | The vertical offset of the morph shape above the bottom navigation (by default 8dp) |



## License
    Copyright 2018 Tommy Buonomo
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
        http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

