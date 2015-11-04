# Search Center 1.6

한국어를 사용하신다면 아래에서 한국어 버전을 선택해 주세요.  
[한국어 버전](https://github.com/peterSupport/SearchCenterSupport/blob/master/readme16.md)  
If you need support, please contact the developer.  
[Contact](mailto:searchcenterapp@gmail.com)  

Thanks!

## Note
**It is possible that your search history remains within this app even though you are using privacy mode in Safari. You can swipe and delete each search history, or you may set 0 for the amount of history term to save. There is a button on the side menu that deletes the search history.**

## Release Note
- App Icon Changed  
- Bluetooth Keyboard Shortcut: Normal Search, Continuous Search, Close the Result, Designated Search Actions for Numeric Keys, Various Option Toggles, etc..  
- Buttons to Change Icon Size are Added  
- iPad Pro Support  
- 3D Touch: Peek & Pop, Quick Action  
- You can Clear the Main Search Term Textbox with a Left Swipe Gesture.  
- Today Widget Added  
- Icon Size is Increased for 4.7 inch Devices  
- Various Bug Fixes and Improvements  

## Basic Gestures
![MainView01](http://i.imgur.com/vgeUgsn.png)

### Top Area
Tap: Scrolls to either the default search action or the last used search action according to the setting.   
Double-Tap: Shows/Hides search terms used in past.  
Double-Tap & Hold: Puts the last used search term in the text field.  
Long-Tap: Launches either default search action or continuous search action that is opposite from the corresponding setting.  
Horizontal Swipe: Moves cursor in the search term text field.  

### Search Term Text Field
Horizontal Swipe: Moves cursor in the search term text field.  

### Search Action Area
Vertical Swipe: Scrolls through the search actions.  
Horizontal Swipe: Shows/Hides side menu.  
Long-Tap on Search Action: You can Drag&Drop icons. Drop Zone will be displayed where you can drop the icon to do some actions with the search action.  
Swipe Left: Clears the search term text field if side menu is not displayed.  

### Done Button on the Keyboard
Done Button on the keyboard launches either the default search action or the continuous search action. You can set which on the side menu.  
Default actions and continuous actions(the search action used last time) are marked with star-shaped icon and bookmark-shaped icon, respectively. The icon under the title "Search Center" in the Top Area represents the search action that will be launched when you hit the done button on the keyboard.  

### Drag&Drop
![DragAndDropb](http://i.imgur.com/xXPwFJC.png)
Long tapping one of your search actions initiates Drag&Drop mode. Using Drag&Drop gesture, you can rearrange your search actions easily.  
While you are dragging one of your search actions, Drop Zone will be presented over the top area.  
Drop Zone has four sections in which you can "Drop" the icon under your finger to launch the action of the area.  For example, if you dropped Wikipedia search action in the Delete section of the Drop Zone, Wikipedia search action will be deleted from your search actions collection.  
* Set Default: Sets the search action default, marking the icon with star.  
* Edit: Presents the scene where you can edit the icon, title, and URL of the search action.  
* Delete: Deletes the search action from your collection.  
* Duplicate: Makes a copy of the search action.  

## Default Search and Continuous Search

![Markers](http://i.imgur.com/mNTxApZ.png)  

### Default Search
The search action set as default will be marked with star shaped icon. Default search action will be launched with the term you typed if the icon in the top area is star shaped icon, which you can set in the side menu.  
**If you have not set an search action as default, nothing will happen when you press the done button.**  

### Continuous Search
The search action marked with bookmark shaped icon is the search action used lately. If you have set options accordingly, pressing done button will launch this search action repeatedly, and continuously.  

## Adding a New Search Action
![addVC](http://i.imgur.com/bXrShtl.png)  
This scene will be presented when you creating a new search action or editing an existing one.  
You can add a new search action by tapping the "+" button on the top right hand corner of the main screen. This scene has a few gestures you can use conveniently.  
* Tap in the blank area: Dismisses the keyboard.  
* Double-Tap in the blank area: Presents URL Templates.  
* Horizontal Swipe: Moves the cursor in the text field.  

### Set an Icon for the Search Action
![addnewicon](http://i.imgur.com/eSRZelH.png)  
You can set an icon for the search action by tapping the black rectangle on the top of the screen. 
* Photo Library: You can select an icon from your photo collection.  
* Image URL: Copy an URL of the image you like, and paste it here to get the image from the internet.  
* App Store Link: You can set the icon of an app from the App Store as the icon of the Search Action. Please see below to know how.  
* Load Icons: Use one of the icons of existing search actions.  

#### How to Get the Icon of an App?
![appStore01](http://i.imgur.com/YseMwfn.png)  
![appStore02](http://i.imgur.com/EeDqBJM.png)  
In the app page you like in the App Store, press the share button. Then, press the copy link button on the share sheet.  
Now you have the link for the app, please paste it in the text field that is displayed when you had selected "App Store Link" from the above.  
The link would look like this:  

	Search Center - Search with One Tap by HyeonChol Jang
	https://appsto.re/us/v63-8.i 

### URL Template
You may use your own URL for the search action, or choose one of the templates if you are not sure.  
![temp01](http://i.imgur.com/BjvZISY.png)  

Please either tap twice fast in blank area of the scene above, or press the Templates button on the bottom to see the URL Templates screen.  Also, press the list button on the top right hand corner next to the save button to call the teamplates screen.  
URL Templates will be displayed automatically when you are creating a new search action.  

![temp02](http://i.imgur.com/AwGWWoX.png)  
Select one of the examples, set an icon(or not), edit the title and URL if you'd like, and press the save button on the top right hand corner of the screen.  

If you'd like to suggest some new features or request new examples, please contact the developer.  
**Not all requests can be implemented if there is no API, it is not permitted by the provider, or etc..**  

### How to Edit URL?
There are two tags to be used when editing an URL.  
1. {query}: This tag will be replaced with the search term you typed in when you launch this search action.  
2. {location}: This tag will be replaced with the GPS coordinates in format of "latitude,longtitude".  

For example, suppose that you search a lot about recipes on the internet. You will have to type in "recipe" repeatedly. However, if you edit the google search url a little bit, you no longer have to do this over and over again.  
Google search URL is `http://www.google.com/search?q={query}` and the `{query}` will be replaced by the search term you use. So, you need to add "recipe" after `{query}` tag. The result is:  

	http://www.google.com/search?q={query}+recipe
	
The plus sign represents a white space which is very useful when manipulating URLs.  Now if you save this search action with the edited URL above, you just need to type in the name of the cuisine. Search Center will present you with the search result of `spagetti recipe`, for instance.  

## 3D Touch
Peek & Pop and Quick Action is supported on the 3D Touch-Enabled devices.  
You can Peek the search result by pressing hard on a search action.  If you press harder, the search result will Pop into the full screen search result.  
![PeeknPop](http://i.imgur.com/NNnhOlA.jpeg)  
Quick Actions are accessible by pressing hard the app icon from the home screen. You can choose the quick actions from the side menu.  
![QuickAction](http://i.imgur.com/xDtXp1t.jpeg) 

## URL Scheme
If you use Launch Center or Luancher, or an similar app, you may use `searchcenter:///`.

## Bluetooth Keyboard Shortcuts
![Shortcut01](http://i.imgur.com/ffkdTPx.png)  
![Shortcut02](http://i.imgur.com/ESEmqs2.png)  

In iOS 9, you will be presented with the list of shortcuts you may use if you press and hold command key. Basically, `command + w` will dismiss the search result.  

**If you have used keyboard in the web search result, keyboard shortcuts would not work**







