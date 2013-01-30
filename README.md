#PSGradientButtons
A collection of buttons for use in Android applications. All buttons are in the form of xml-selectors and don't require any images. The advantage of using XML Drawables is that they automatically adjust to the correct size.

#Usage
All graphical assets for the buttons are stored in Drawable folder and can get directly accessed as Drawables in XML via @drawable/filename whereby filename is the filename without extension. For example to acceces the ps__button_github.xml file, you would use @drawable/ps__button_github. 

To use the drawables, just add the xml drawable as the background for your button in layout.

```
<Button
  ..
  android:background="@drawable/ps__button_github"
  ..
   />
```

Or set them programmatically using [setBackgroundResource](http://developer.android.com/reference/android/view/View.html#setBackgroundResource%28int%29).

```
myButton.setBackgroundResource(R.drawable.ps__button_github);
```

There are two ways to include the buttons in your project: 

1. Copy the xml drawables into your project: This is probably the simplest way to start using the buttons in your project. All you need to do is copy the xml drawable that you would like to use in `res/drawable/` directory in your project.
2. Include GradientButtons as a library project into your project: If you would like to try out several of the buttons and don't feel like copying them into your project, you can also include PSGradientButtons as a library project. Just follow these steps: 

* Import PSGradientButtons into eclipse as an Android project. `File` -> `Import` -> `Existing Android code into Workspace`.
* Right click on PSGradientButtons and go to `Properties` (`⌘I` or `^I`) -> `Android` and make sure that `Is Library` is checked.
* Right click on your project and go to `Properties` (`⌘I` or `^I`) -> `Andaroid` and `Add` PSGradientButtons as a library.
* Start using the xml drawables.

#License
Copyright © [Sapan Diwakar](http://sapandiwakar.in) and [Pulkit Goyal](http://pulkitgoyal.in)

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

See the License for the specific language governing permissions and limitations under the License.

Authors: 
Sapan Diwakar (diwakar.sapan@gmail.com)
Pulkit Goyal (pulkit110@gmail.com)